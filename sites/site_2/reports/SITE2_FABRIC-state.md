# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 128 | 104 | 0 | 24 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s2-leaf1 | 19 | 15 | 0 | 4 | - | Hardware |
| s2-leaf2 | 19 | 15 | 0 | 4 | - | Hardware |
| s2-leaf3 | 19 | 15 | 0 | 4 | - | Hardware |
| s2-leaf4 | 19 | 15 | 0 | 4 | - | Hardware |
| s2-spine1 | 26 | 22 | 0 | 4 | - | Hardware |
| s2-spine2 | 26 | 22 | 0 | 4 | - | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| Connectivity | 28 | 28 | 0 | 0 |
| Hardware | 24 | 0 | 0 | 24 |
| Interfaces | 64 | 64 | 0 | 0 |
| MLAG | 6 | 6 | 0 | 0 |
| System | 6 | 6 | 0 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s2-leaf2 Ethernet1 | PASS | - |
| 2 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s2-spine1 Ethernet2 | PASS | - |
| 3 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s2-spine2 Ethernet2 | PASS | - |
| 4 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s2-leaf2 Ethernet6 | PASS | - |
| 5 | s2-leaf1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 6 | s2-leaf1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 7 | s2-leaf1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 8 | s2-leaf1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 9 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s2-leaf2_Ethernet1 = 'up' | PASS | - |
| 10 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S2-SPINE1_Ethernet2 = 'up' | PASS | - |
| 11 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S2-SPINE2_Ethernet2 = 'up' | PASS | - |
| 12 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - s2-host1_eth1 = 'up' | PASS | - |
| 13 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s2-leaf2_Ethernet6 = 'up' | PASS | - |
| 14 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s2-leaf2_Po1 = 'up' | PASS | - |
| 15 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po2 = 'up' | PASS | - |
| 16 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - s2-host1 = 'up' | PASS | - |
| 17 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 18 | s2-leaf1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 19 | s2-leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 20 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s2-leaf1 Ethernet1 | PASS | - |
| 21 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s2-spine1 Ethernet3 | PASS | - |
| 22 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s2-spine2 Ethernet3 | PASS | - |
| 23 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s2-leaf1 Ethernet6 | PASS | - |
| 24 | s2-leaf2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 25 | s2-leaf2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 26 | s2-leaf2 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 27 | s2-leaf2 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 28 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s2-leaf1_Ethernet1 = 'up' | PASS | - |
| 29 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S2-SPINE1_Ethernet3 = 'up' | PASS | - |
| 30 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S2-SPINE2_Ethernet3 = 'up' | PASS | - |
| 31 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - s2-host1_eth2 = 'up' | PASS | - |
| 32 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s2-leaf1_Ethernet6 = 'up' | PASS | - |
| 33 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s2-leaf1_Po1 = 'up' | PASS | - |
| 34 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po2 = 'up' | PASS | - |
| 35 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - s2-host1 = 'up' | PASS | - |
| 36 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 37 | s2-leaf2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 38 | s2-leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 39 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s2-leaf4 Ethernet1 | PASS | - |
| 40 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s2-spine1 Ethernet4 | PASS | - |
| 41 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s2-spine2 Ethernet4 | PASS | - |
| 42 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s2-leaf4 Ethernet6 | PASS | - |
| 43 | s2-leaf3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 44 | s2-leaf3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 45 | s2-leaf3 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 46 | s2-leaf3 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 47 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s2-leaf4_Ethernet1 = 'up' | PASS | - |
| 48 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S2-SPINE1_Ethernet4 = 'up' | PASS | - |
| 49 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S2-SPINE2_Ethernet4 = 'up' | PASS | - |
| 50 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - s2-host2_eth1 = 'up' | PASS | - |
| 51 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s2-leaf4_Ethernet6 = 'up' | PASS | - |
| 52 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s2-leaf4_Po1 = 'up' | PASS | - |
| 53 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po4 = 'up' | PASS | - |
| 54 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - s2-host2 = 'up' | PASS | - |
| 55 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 56 | s2-leaf3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 57 | s2-leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 58 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s2-leaf3 Ethernet1 | PASS | - |
| 59 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s2-spine1 Ethernet5 | PASS | - |
| 60 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s2-spine2 Ethernet5 | PASS | - |
| 61 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s2-leaf3 Ethernet6 | PASS | - |
| 62 | s2-leaf4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 63 | s2-leaf4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 64 | s2-leaf4 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 65 | s2-leaf4 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 66 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s2-leaf3_Ethernet1 = 'up' | PASS | - |
| 67 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S2-SPINE1_Ethernet5 = 'up' | PASS | - |
| 68 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S2-SPINE2_Ethernet5 = 'up' | PASS | - |
| 69 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - s2-host2_eth2 = 'up' | PASS | - |
| 70 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s2-leaf3_Ethernet6 = 'up' | PASS | - |
| 71 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s2-leaf3_Po1 = 'up' | PASS | - |
| 72 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - SPINES_Po4 = 'up' | PASS | - |
| 73 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - s2-host2 = 'up' | PASS | - |
| 74 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 75 | s2-leaf4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 76 | s2-leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 77 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s2-spine2 Ethernet1 | PASS | - |
| 78 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s2-leaf1 Ethernet2 | PASS | - |
| 79 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s2-leaf2 Ethernet2 | PASS | - |
| 80 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet4 - Remote: s2-leaf3 Ethernet2 | PASS | - |
| 81 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: s2-leaf4 Ethernet2 | PASS | - |
| 82 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s2-spine2 Ethernet6 | PASS | - |
| 83 | s2-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 84 | s2-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 85 | s2-spine1 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 86 | s2-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 87 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s2-spine2_Ethernet1 = 'up' | PASS | - |
| 88 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S2-LEAF1_Ethernet2 = 'up' | PASS | - |
| 89 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S2-LEAF2_Ethernet2 = 'up' | PASS | - |
| 90 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - S2-LEAF3_Ethernet2 = 'up' | PASS | - |
| 91 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - S2-LEAF4_Ethernet2 = 'up' | PASS | - |
| 92 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s2-spine2_Ethernet6 = 'up' | PASS | - |
| 93 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Loopback0 - Router_ID = 'up' | PASS | - |
| 94 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s2-spine2_Po1 = 'up' | PASS | - |
| 95 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - RACK1_Po2 = 'up' | PASS | - |
| 96 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - RACK2_Po2 = 'up' | PASS | - |
| 97 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan30 - Thirty = 'up' | PASS | - |
| 98 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan40 - Forty = 'up' | PASS | - |
| 99 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4093 - MLAG_PEER_L3_PEERING = 'up' | PASS | - |
| 100 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 101 | s2-spine1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 102 | s2-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 103 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s2-spine1 Ethernet1 | PASS | - |
| 104 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s2-leaf1 Ethernet3 | PASS | - |
| 105 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s2-leaf2 Ethernet3 | PASS | - |
| 106 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet4 - Remote: s2-leaf3 Ethernet3 | PASS | - |
| 107 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: s2-leaf4 Ethernet3 | PASS | - |
| 108 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s2-spine1 Ethernet6 | PASS | - |
| 109 | s2-spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 110 | s2-spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 111 | s2-spine2 | Hardware | VerifyTemperature | Verifies the device temperature. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 112 | s2-spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 113 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet1 - MLAG_PEER_s2-spine1_Ethernet1 = 'up' | PASS | - |
| 114 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet2 - S2-LEAF1_Ethernet3 = 'up' | PASS | - |
| 115 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet3 - S2-LEAF2_Ethernet3 = 'up' | PASS | - |
| 116 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet4 - S2-LEAF3_Ethernet3 = 'up' | PASS | - |
| 117 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet5 - S2-LEAF4_Ethernet3 = 'up' | PASS | - |
| 118 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Ethernet6 - MLAG_PEER_s2-spine1_Ethernet6 = 'up' | PASS | - |
| 119 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Loopback0 - Router_ID = 'up' | PASS | - |
| 120 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel1 - MLAG_PEER_s2-spine1_Po1 = 'up' | PASS | - |
| 121 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel2 - RACK1_Po2 = 'up' | PASS | - |
| 122 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Port-Channel4 - RACK2_Po2 = 'up' | PASS | - |
| 123 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan30 - Thirty = 'up' | PASS | - |
| 124 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan40 - Forty = 'up' | PASS | - |
| 125 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4093 - MLAG_PEER_L3_PEERING = 'up' | PASS | - |
| 126 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the status of the provided interfaces. | Interface Vlan4094 - MLAG_PEER = 'up' | PASS | - |
| 127 | s2-spine2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 128 | s2-spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
