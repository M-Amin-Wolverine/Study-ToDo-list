# 📡 Awesome Telco 🚀

A curated list of telco resources and projects.  
Consult [awesome-5g](https://github.com/calee0219/awesome-5g) for 5G specific projects, which is probably more up to date on the matter than this one.  

⭐ **Updated for 2025: Fresh insights from OSS trends, AI-driven innovations, and cloud-native shifts!**  

## 📋 Contents

- [SIM: USIM, SIM, eSIM](#simcards) 💳
- [UE: phones, modems apps](#ue) 📱
- [RAN: 2G, 3G, 4G, 5G](#ran) 📡
- [Core: EPC, MME, SGW, PGW](#core) 🏗️
- [Interco: IMS, SBC, Diameter](#interco) 🔗
- [Protocols: Libraries, Frameworks](#protocols) ⚙️
- [Satellite Communication: Monitoring and tooling](#satcom) 🛰️
- [Infrastructure: SDN and NFV management software](#infrastructure) ☁️
- [Orchestration: Automation and integration software](#orchestration) 🎛️
- [Lab: tooling for telco labs](#lab) 🧪
- [Testing: TTCN3 and others testing frameworks](#testing) 🧪
- [Security: Papers and talks around telco security](#security) 🔒
- [Blogs: Telco-related personal blogs](#blogs) 📝
- [Organizations: Orgs and forums working on telcos hardware/software](#organizations) 👥
- [Docs: Documentations and standards](#docs) 📚
- [Decks: Powerpoints and great slides](#slides) 📊
- [Tweets: Relevant tweets and link to social networks](#tweets) 🐦
- [Issues: interesting issues on bugtrackers](#issues) 🐛
- [Mailing-lists: ML, slack and other forums](#mailing-lists) 💬
- [Commercial: Services around open source tech](#commercial) 💼
- [6G: Emerging projects and resources](#6g) 🌌

## 💳 SIMCards

Tools and projects for SIM/USIM/eSIM management, programming, and emulation.  

- [PySIM](https://osmocom.org/projects/pysim/wiki) - Tools to read, explore, decode, and program SIM/USIM/ISIM cards. Ideal for managing sysmocom cards.  
- [sysmoISIM-SJA5](https://www.sysmocom.de/products/sim/sysmoisim-sja5/) - Programmable SIM/UICC/USIM/ISIM card supporting 3GPP Release 17 for lab/research.  
- [SIMTrace2](https://osmocom.org/projects/simtrace2) - Hardware/firmware for tracing phone-SIM communication; supports ISO7816 emulation.  
- [SIMTester](https://opensource.srlabs.de/projects/simtester) - Assesses SIM card security (cryptanalytic and application attack surfaces).  
- [Njiwa - M2M UICC](https://github.com/brucedchen1991/njiwa) - GSMA Embedded SIM Remote Provisioning Manager for M2M devices (fork).  
- [LPAd SM-DP+ Connector](https://github.com/Truphone/LPAd_SM-DPPlus_Connector) - Local Profile Assistant for Device (LPAd) for SM-DP+ connectivity.  
- [sysmo-usim-tool](https://gitea.sysmocom.de/sysmocom/sysmo-usim-tool) - Utility for sysmoUSIM/sysmoISIM proprietary bits management.  
- [GlobalPlatformPro](https://github.com/martinpaljak/GlobalPlatformPro) - Command-line tool to load and manage SIM applets on JavaCards.  
- [ARA-M Applet](https://github.com/bertrandmartel/aram-applet) - ARA-M implementation for JavaCards by Bertrand Martel.  
- [CoIMS_wiki](https://github.com/herlesupreeth/CoIMS_Wiki) - Guide for overriding IMS settings to enable VoLTE/VoWiFi. [CoIMS app](https://play.google.com/store/apps/details?id=com.sherle.coims).  
- [HelloSTK2](https://github.com/mrlnc/HelloSTK2) - Guide for building/installing SIM-Toolkit applets.  
- [Generic-eUICC-Test-Profile](https://github.com/GSMATerminals/Generic-eUICC-Test-Profile-for-Device-Testing-Public) - Normalizes Test Profiles for embedded UICCs for standardized testing.  

## 📱 UE

### 4G 📶

- [srsUE](https://github.com/srslte/srslte) - 4G UE modem part of srsLTE project.  
- [srsUE PR external NAS](https://github.com/srsLTE/srsLTE/pull/474) - PR for external NAS message injection in srsLTE.  
- [OAI UE](https://gitlab.eurecom.fr/oai/openairinterface5g/wikis/home) - Open Air Interface 4G eNB/5G gNB for SDR radios.  
- [Amarisoft](https://www.amarisoft.com) - Commercial UE Emulator by Amarisoft, based on Bellard’s LTE work.  
- [LTE-CellScanner](https://github.com/Evrytania/LTE-Cell-Scanner) - Tools to locate/track LTE basestation cells with low-performance RF.  
- [LTE-CellScanner-SDR-X](https://github.com/JiaoXianjun/LTE-Cell-Scanner) - OpenCL-accelerated TDD/FDD LTE Scanner for rtlsdr/hackRF/bladeRF.  
- [S1APTester](https://github.com/facebookexperimental/S1APTester) - Simulates S1AP functionality for LTE network testing.  
- [UERANSIM](https://github.com/aligungr/UERANSIM) - 5G UE/gNodeB simulator for 5G Core testing and study.  
- [PacketRusher](https://github.com/HewlettPackard/PacketRusher) - High-performance 5G UE/gNB simulator and load tester.  
- [corescope](https://github.com/srsran/corescope) - Combines gNodeB/UE without radio transmission.  

### 2G 📡

- [OsmocomBB](https://osmocom.org/projects/baseband/wiki) - Open Source 2G Mobile Station with TI Calypso chipset; SDR PHY WIP.  
- [FreeCalypso](https://www.freecalypso.org/) - Software from leaked TI Calypso source code.  
- [OpenBTS](http://openbts.org) - 2G BTS with SDR radios.  
- [YateBTS](https://wiki.yatebts.com/index.php/Main_Page) - 2G BTS with SDR radios.  
- [OsmoTRX](https://osmocom.org/projects/osmotrx) - OpenBTS transceiver fork for SDR radios.  
- [OsmoBTS](https://osmocom.org/projects/osmobts) - Open Source GSM BTS with A-bis/IP interface.  

### Diagnostics, Monitor mode 🔍

- [SCAT](https://github.com/fgsect/scat) - Parses Qualcomm/Samsung baseband diagnostic messages, generates GSMTAP packets.  
- [QCSuper](https://github.com/P1sec/QCSuper) - Captures raw 2G/3G/4G radio frames from Qualcomm phones/modems.  
- [Network Signal Guru](http://m.qtrun.com/en/) - Android app parsing QC modem Diag output for engineering data.  
- [Snoopsnitch](https://opensource.srlabs.de/projects/snoopsnitch) - Collects network data via passive/active tests on rooted Android using DIAG.  
- [Diag-parser](https://github.com/moiji-mobile/diag-parser) - Converts Qualcomm DIAG 2G/3G/4G messages to GSMTAP for Wireshark.  
- [XGoldmon](https://github.com/2b-as/xgoldmon) - Converts USB logging from Intel/Infineon XGold baseband phones.  
- [Modmobmap](https://github.com/PentHertz/Modmobmap) - Maps 2G/3G/4G networks in real-time with smartphones.  
- [Modmobjam](https://github.com/PentHertz/Modmobjam) - Smart jamming POC powered by Modmobmap.  

## 📡 RAN

### RRH 📡

- [O-RAN Software and seed code](https://o-ran-sc.org) - O-RAN Software Community for RAN software; [LF video](https://www.youtube.com/watch?v=iJyb0pCWDKo).  
- [SD-RAN](https://opennetworking.org/sd-ran/) - ONF’s split RAN with near real-time RIC and xApps.  
- [Nokia O-RAN](https://www.nokia.com/about-us/newsroom/articles/nokia-open-ran/) - Nokia’s contributions to O-RAN standards and solutions.  
- [Radisys O-RAN](https://www.radisys.com/solutions/open-ran) - Open RAN solutions for scalable deployments.  
- [Parallel Wireless O-RAN](https://www.parallelwireless.com/products/open-ran/) - Open RAN for global connectivity.  
- [FlexRAN](https://www.intel.com/content/www/us/en/developer/topic-technology/edge-5g/tools/flexran.html) - Intel’s reference software for O-RAN.  

### 5G 🌐

- [srsRAN_Project](https://github.com/srsran/srsRAN_Project) - ORAN-native 5G RAN solution.  
- [OAI NR](https://gitlab.eurecom.fr/oai/openairinterface5g/wikis/5g-nr-development-and-releases) - 5G NR branch of OAI; [weekly updates](https://trello.com/c/XBVaaHIO/26-5g-nr).  
- [UERANSIM](https://github.com/aligungr/UERANSIM) - 5G UE/gNodeB simulator for 5G Core testing.  
- [Software gNB for free5GC](https://github.com/Srajdax/gnb) - gNB built on free5GC CN patterns.  
- [gnbsim](https://github.com/AlohaLuo/gnbsim-backup) - 5G SA gNB/UE (R16) simulator for 5GC testing.  
- [5G-tools.com](https://5g-tools.com/) - Software tools for 5G/4G wireless networks.  
- [corescope](https://github.com/srsran/corescope) - gNodeB/UE combo without radio transmission.  
- [my5G-RANTester](https://github.com/my5G/my5G-RANTester) - gNB/UE simulator for 3GPP testing and 5G core stress.  
- [free5GRAN](https://github.com/free5G/free5GRAN) - Open-source 5G RAN; decodes MIB/SIB1, cell scanner in SA mode.  
- [pfm](https://github.com/arv-sajeev/pfm) - gNB-CU-UP prototype using DPDK for packet processing.  
- [PacketRusher](https://github.com/HewlettPackard/PacketRusher) - High-performance 5G UE/gNB simulator and load tester.  
- [py3gpp](https://github.com/catkira/py3gpp) - Python package for 5G-NR simulations.  

### 4G 📶

- [OAI eNB/gNB](https://gitlab.eurecom.fr/oai/openairinterface5g/wikis/home) - 4G eNB/5G gNB for SDR radios.  
- [srsLTE](https://github.com/srslte/srslte) - 4G eNB for SDR radios.  
- [LTE-ciphercheck](https://github.com/mrlnc/LTE-ciphercheck) - srsLTE derivative to check LTE cipher configs with SDR.  
- [OpenLTE](http://openlte.sourceforge.net) - Open source 3GPP LTE implementation.  
- [Cisco 4G nFAPI](https://github.com/cisco/open-nFAPI) - Small Cell Forum’s nFAPI for LTE L1-L2+ connectivity.  
- [CrocodileHunter](https://github.com/EFForg/crocodilehunter) - Hunts fake eNodeBs by analyzing 4G broadcasts.  
- [eNB s1 emulator](https://github.com/fasferraz/eNB) - Python3 eNB emulator for MME/SGW; simulates EMM/ESM.  
- [radisys_lte_enb_for_qualcomm_fsm9955](https://github.com/laf0rge/radisys_lte_enb_for_qualcomm_fsm9955) - Radisys LTE eNB for Qualcomm FSM9955.  

### 3G 📡

- [OpenUMTS](https://github.com/RangeNetworks/OpenBTS-UMTS) - 3G NodeB implementation.  
- [openbts-UMTS](https://github.com/PentHertz/OpenBTS-UMTS) - Updated OpenBTS-UMTS with 2023 dependencies; [Docker](https://hub.docker.com/r/penthertz/openbts-umts).  
- [OsmoHNodeB](https://osmocom.org/projects/osmo-hnodeb) - Upper layers (RANAP/RUA/HNBAP/GTP/RTP) for hNodeB.  
- [YateBTS](https://wiki.yatebts.com/index.php/Main_Page) - Supports 3G alongside 2G with SDR radios.  
- [OpenBSC](https://osmocom.org/projects/osmobsc/wiki) - Supports 3G via IuCS/IuPS interfaces.  
- [srsRAN](https://github.com/srsran/srsRAN) - Includes 3G support for SDR-based NodeB.  

### 2G 📶

- [OpenBTS](http://openbts.org) - 2G BTS with SDR radios.  
- [YateBTS](https://wiki.yatebts.com/index.php/Main_Page) - 2G BTS with SDR radios.  
- [OsmoTRX](https://osmocom.org/projects/osmotrx) - OpenBTS transceiver fork for SDR.  
- [OsmoBTS](https://osmocom.org/projects/osmobts) - Open Source GSM BTS with A-bis/IP.  
- [OsmoPCU](https://osmocom.org/projects/osmopcu/wiki/OsmoPCU) - Open source GPRS PCU with Gb/IP; supports OsmoBTS/Ericsson RBS.  
- [OsmoBSC](https://osmocom.org/projects/osmobsc/wiki) - Open Source BSC with Abis/E1/IP; supports multiple BTS models.  

### PHY 🔧

- [gr-osmoSDR](https://osmocom.org/projects/gr-osmosdr) - GNU Radio I/O block for SDR devices (FUNcube, RTL-SDR, HackRF, etc.).  
- [USRP B210](https://www.ettus.com/all-products/UB210-KIT/) - SDR kit for SDR-based modem implementations.  
- [Kalibrate](https://github.com/steve-m/kalibrate-rtl) - Scans GSM base stations; calculates oscillator offset.  
- [CSDR](https://github.com/simonyiszk/csdr) - Command-line DSP tool for SDR.  
- [srsRAN](https://github.com/srsran/srsRAN) - PHY layer support for 4G/5G SDR implementations.  
- [BladeRF](https://www.nuand.com/) - SDR platform for PHY layer testing in telco setups.  

## 🏗️ Core

### 5G 🌐

- [Open5GS](https://open5gs.org) - 5G/R14 4G EPC core with MME, HSS, SGW, PGW, PCRF, UPF, SMF, NRF. [GitHub](https://github.com/open5gs).  
- [OAI 5GCN](https://gitlab.eurecom.fr/oai/cn5g) - 3GPP-compliant 5G SA Core Network by EURECOM.  
- [travelping-vpp](https://github.com/travelping/vpp) - UPF plugins for GTP-U (3GPP TS 23.214/29.244 R15) in VPP.  
- [IITB 5G SBA PoC](https://github.com/iithnewslab/SBA-gRPC-5G) - Prototyping 5G Core SBA using NFV; [paper](https://github.com/iithnewslab/SBA-gRPC-5G/blob/master/Presentation_Netsoft19_gRPC_5G.pdf).  
- [Free5GC](https://www.free5gc.org/) - Open-source 5G core in Golang; [APER](https://github.com/free5gc/aper), [AMF](https://github.com/free5gc/amf).  
- [5GC Swagger APIS](https://github.com/jdegre/5GC_APIs) - RESTful APIs for 5G Core NFs (R16).  
- [5G GTP kernel driver](https://github.com/PrinzOwO/gtp5g) - Linux kernel module for 5G GTP-U with PFCP IEs.  
- [UPF-EPC](https://github.com/omec-project/upf-epc) - Revised ngic-rtc dp with BESS dataplane.  
- [OpenUPF](https://github.com/5GOpenUPF/openupf) - 3GPP R16 open source 5G UPF.  
- [Katana Slice Manager](https://github.com/medianetlab/katana-slice_manager) - Controls network devices for slice management.  

### 4G 📶

- [OAI EPC](https://github.com/OPENAIRINTERFACE/openair-cn/wiki) - MME and HSS from OAI projects.  
- [NextEPC](https://nextepc.org) - R13 4G EPC with MME, HSS, SGW, PGW, PCRF. [GitHub](https://github.com/nextepc/).  
- [Magma](https://github.com/facebookincubator/magma) - Core with access gateway (MME+P/SGW), federation for auth/billing.  
- [C3PO](https://github.com/omec-project/c3po) - HSS, CDF, CTF, PCRF with Cassandra DB and SGX; from OMEC.  
- [NGIC-RTC](https://github.com/omec-project/ngic-rtc) - CUPS-based EPC SGW/PGW (3GPP TS23501); from OMEC.  
- [OpenMME](https://github.com/omec-project/openmme) - MME EPC S1 front end from OMEC.  
- [srsEPC](https://github.com/srslte/srslte) - Lightweight LTE core with MME, HSS, S/P-GW.  
- [corenet](https://github.com/mitshell/corenet) - Minimal 3G/LTE EPC using Pycrate.  

### 3G 📡

- [OsmoHNBGW](https://osmocom.org/projects/osmohnbgw) - HNB-GW with Iuh, IuCS, IuPS for femtocell aggregation.  
- [OpenUMTS](https://github.com/RangeNetworks/OpenBTS-UMTS) - 3G core support via IuCS/IuPS.  
- [OsmoMSC](https://osmocom.org/projects/osmomsc/wiki) - MSC with IuCS support for 3G.  
- [OsmoSGSN](https://osmocom.org/projects/osmosgsn/wiki) - SGSN with IuPS for 3G support.  
- [OsmoHLR](https://osmocom.org/projects/osmo-hlr/wiki/OsmoHLR) - HLR with GSUP for 3G core.  
- [OsmoMGW](https://osmocom.org/projects/osmo-mgw/wiki) - MGW for 3G user plane routing.  

### 2G + 3G 📶

- [OsmoMSC](https://osmocom.org/projects/osmomsc/wiki) - MSC with 3GPP AoIP/IuCS/GSUP interfaces.  
- [OsmoHLR](https://osmocom.org/projects/osmo-hlr/wiki/OsmoHLR) - HLR with GSUP for OsmoMSC/SGSN.  
- [OsmoSGSN](https://osmocom.org/projects/osmosgsn/wiki/OsmoSGSN) - SGSN with Gb/IP, IuCS, GSUP, GTP Gp.  
- [OsmoGGSN](https://osmocom.org/projects/openggsn/wiki) - GGSN with Gp to SGSN, Gi to IP network.  
- [OsmoMGW](https://osmocom.org/projects/osmo-mgw/wiki) - MGW for RTP routing; supports LCLS/IuFP.  
- [OsmoSTP](https://osmocom.org/projects/osmo-stp/wiki) - STP for SS7 routing via M3UA/SUA/SCCPlite.  

### OSS/BSS 🛠️

- [Sigscale OCS](https://github.com/sigscale/ocs) - 3GPP AAA server for DIAMETER/RADIUS subscriber auth/accounting.  
- [Bodastage CE](http://www.bodastage.org) - Telecom network management for RAN providers. [GitHub](https://github.com/bodastage/bts-ce).  
- [NextOSS](https://github.com/NextOSS/awesome-oss) - OSS/BSS solutions for telecom.  
- [OpenNMS](https://www.opennms.com/) - Network monitoring for telecom OSS.  
- [Apache Camel](https://camel.apache.org/) - Integration framework for OSS/BSS workflows.  
- [ONAP](https://www.onap.org/) - OSS automation platform for telco services.  

## 🔗 Interco

### SBC, IMS 🌐

- [Freeswitch](https://freeswitch.org/confluence/display/FREESWITCH/Python_SBC) - SIP stack usable as SBC.  
- [IMS Clearwater](http://www.projectclearwater.org) - Open source IMS implementation.  
- [Kamailio](https://www.kamailio.org) - SIP stack for VoLTE/SBC.  
- [go-eventsocket](https://github.com/fiorix/go-eventsocket) - FreeSWITCH Event Socket library for Go.  
- [Asterisk](https://www.asterisk.org/) - Open source PBX and telephony toolkit.  
- [Homer](https://github.com/sipcapture/homer) - Open-source SIP/VoIP packet capture and monitoring.  

### SS7 🔒

- [Restcomm SS7](https://github.com/restcomm/jss7) - Java SS7 stack for legacy equipment.  
- [SigFW](https://github.com/P1sec/SigFW) - Signaling Firewall for SS7/Diameter filtering.  
- [yate](https://github.com/yatevoip/yate) - Telephony engine with MTP2/3, M2PA/UA,руса
- [go-m3ua](https://github.com/wmnsk/go-m3ua) - Package m3ua provides easy and painless handling of M3UA protocol in pure Golang.
- [go-sccp](https://github.com/wmnsk/go-sccp) - Package sccp provides simple and painless handling of SCCP(Signaling Connection Control Part) in SS7/SIGTRAN stack, implemented in the Go Programming Language.
- [libosmo-sccp](https://git.osmocom.org/libosmo-sccp/) - SCCP Library
- [go-tcap](https://github.com/wmnsk/go-tcap) - Package tcap provides simple and painless handling of TCAP(Transaction Capabilities Application Part) in SS7/SIGTRAN protocol stack.
- [openss7](http://www.openss7.org/) - An opensource development project (called OpenSS7) to provide a robust and GPL'ed SS7, SIGTRAN, ISDN and VoIP stack for Linux and other UN*X operating systems.

### Dataplane acceleration

- [Ligato](https://github.com/ligato/vpp-agent) - Controlplane agent for FD.io VPP
- [FD.io](https://fd.io) - FD.io is a vector processing engine (VPP). VPP processes a number of packets in parallel instead of one at a time thus significantly improving packet throughput.
- [OVS](http://www.openvswitch.org) - Open vSwitch is a production quality, multilayer virtual switch licensed under the open source Apache 2.0 license.
- [DPDK](https://www.dpdk.org) - DPDK is the Data Plane Development Kit that consists of libraries to accelerate packet processing workloads running on a wide variety of CPU architectures. [Vista Creek (FPGA-based baseband accelerator)](https://www.intel.com/content/www/us/en/wireline/products/programmable/applications/nfv.html) support has been added to [DPDK](https://doc.dpdk.org/guides/bbdevs/fpga_lte_fec.html).

### Others

- [open-nFAPI](https://github.com/cisco/open-nFAPI) - Open-nFAPI is implementation of the Small Cell Forum's network functional API or nFAPI for short. nFAPI defines a network protocol that is used to connect a Physical Network Function (PNF) running LTE Layer 1 to a Virtual Network Function (VNF) running LTE layer 2 and above.
- [CSDR](https://github.com/simonyiszk/csdr) - csdr is a command line tool to carry out DSP tasks for Software Defined Radio.
- [OGSLib](https://github.com/open5gs/ogslib) - state machine and utilities functions for NextEPC and Open5gs
- [DiagLibrary](https://github.com/sanjaywave/DiagLibrary) -  a JNI library that implement a DIAG protocol parser under C code to be used under Android or Linux.
- [5G Trace visualizer](https://github.com/telekom/5g-trace-visualizer) - DT set of Python scripts allow you to convert pcap, pcapng or pdml 5G protocol traces (Wireshark, tcpdump, ...) into SVG sequence diagrams.
- [sigshark](https://github.com/2b-as/sigshark) - Sigshark makes working with SS7 TCAP (MAP/CAP) and Diameter signaling pcap files easier. Its features include "flattening" (putting each SCTP chunk in its own packet) and transaction sorting/grouping.
- [ipccdownloader](https://github.com/mrlnc/ipcc-downloader) - Download IPCC Carrier Profiles
- [4g-speed](https://github.com/jake-cryptic/4g-speed) - 4G Theoretical Speed Calculator | FDD & TDD Support

Resources


## Infrastructure

### NFV, Openstack

- [Openstack Kolla](https://github.com/openstack/kolla) - Production ready containers and Ansible tools for deploying an Openstack cluster to run NFV functions.
- [SNAPS-openstack](https://github.com/cablelabs/snaps-openstack) - Openstack deployment to be used on SNAPS booted machine from Cablelabs.
- [OPNFV](https://www.opnfv.org/software/downloads) - The OPNFV project addresses a number of aspects in the development of a consistent virtualisation platform including common hardware requirements, software architecture, MANO and applications.

### Containers, Kubernetes

- [Kubernetes KubeADM](https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm/) - Deployment tool to create Kubernetes cluster.
- [Intel Multus CNI plugin](https://github.com/intel/multus-cni) - Multus CNI is a container network interface (CNI) plugin for Kubernetes that enables attaching multiple network interfaces to pods from Intel.
- [Intel SRVIOV/DPDK CNI plugin](https://github.com/intel/sriov-cni) - SR-IOV CNI plugin works with SR-IOV device plugin for VF allocation for a container.
- [Nokia Danm](https://github.com/nokia/danm/) - TelCo grade network management in a Kubernetes cluster from Nokia.
- [SNAPS-kubernetes](https://github.com/cablelabs/snaps-kubernetes) - Kubernetes deployment to be used on SNAPS booted machine from Cablelabs.
- [Free5GC on kubeCORD](https://github.com/sufuf3/kube5GC) - This project is for deploying Free5GC on kubeCORD.
- [CNCF CNF-Testbed](https://github.com/cncf/cnf-testbed) - The CNCF CNF Testbed provides reference code and test cases for running networking code on Kubernetes and OpenStack using emerging cloud native technologies in the Telecom domain. Provides simulated [network functions](https://github.com/cncf/cnf-testbed/tree/master/examples/network_functions).

### Baremetal management

- [SNAPS-boot](https://github.com/cablelabs/snaps-boot) - Baremetal cluster management solution to prepare for a Openstack or k8s deployment from Cablelabs.
- [MAAS](https://maas.io) - Self-service, remote installation of Windows, CentOS, ESXi and Ubuntu on real servers turns your data center into a bare-metal cloud - Metal As A Service.

## Orchestration

- [5g-sharp-orchestrator](https://github.com/Ethon-Shield/5g-sharp-orchestrator) - tool that serves as a comprehensive wrapper for configuring, deploying and monitoring 5G open-source network components, simplifying the orchestration process.

## Lab

### ready to use testbed (Docker, Vagrant etc.)

- [Open5GS-VoLTE](https://github.com/miaoski/docker_open5gs) - This repository is meant to be a install-and-run lab for Open5GS + Kamailio IMS VoLTE study, a follow-up project of Open5GS Tutorial: VoLTE Setup with Kamailio IMS and Open5GS, which is mainly contributed by Herle Supreeth.
- [Open5GS](https://github.com/herlesupreeth/docker_open5gs) - Docker files to build and run open5gs in a docker by Herle Supreeth.
- [Open5gs-K8s-VyOS](https://dev.to/infinitydon/virtual-4g-simulation-using-kubernetes-and-gns3-3b7k) - This tutorial is about how to deploy a virtual 4G stack using GNS3 and Kubernetes.
- [mobile-env](https://github.com/stefanbschneider/mobile-env) - An open, minimalist Gym environment for autonomous coordination in wireless mobile networks.
- [OpenAICellular](https://openaicellular.github.io/oaic/quickstart.html) - OAIC is an open-source effort led by a consortium of academic institutions to provide fully open-source software architecture, library, and toolset that encompass both the AI controllers (OAIC-C) as well as an AI testing framework (OAIC-T).
- [sample configs](https://github.com/s5uishida/sample_config_misc_for_mobile_network) - Sample Configurations and Miscellaneous for Mobile Network.

### Remote control

- [OpenSTF](https://openstf.io) - Enable remote control of phone over ADB over an HTML5 interfaces.
- [Vyzor](http://vysor.io) - A window to your Android, streaming Android UI through ADB in a Google Chrome Browser app.

### GPS, Time

- [GPS-SDR-SIM](https://github.com/osqzss/gps-sdr-sim) - GPS signal generator with a SDR radio and ephemeris files.
- [Tools for MT3339](https://github.com/f5eng/mt3339-utils) - Ephemeris injector for MT3339-based GPS chipset

## Testing

- [ntt](https://github.com/nokia/ntt) - TTCN-3 test framework.
- [Eclipse Titan TTCN3](https://projects.eclipse.org/projects/tools.titan) - Eclipse Titan is a TTCN-3 compilation and execution environment with an  Eclipse-based IDE.
- [TTCN3vscode](https://github.com/nokia/vscode-ttcn3) - TTCN-3 vs code plugin
- [ixia-c](https://github.com/open-traffic-generator/ixia-c) - Ixia-c is a modern, powerful and API-driven traffic generator designed to cater to the needs of hyperscalers, network hardware vendors and hobbyists alike.
- [Telcometer](https://github.com/itsMohammadHeidari/Telcometer) - Diameter Credit-Control Application Load Testing script powered by [Grafana K6](https://github.com/grafana/k6)

## Security

### Security Exploitation/fuzzing Frameworks

- [SigPloit](https://github.com/SigPloiter/SigPloit) - Telecom Signaling Exploitation Framework - SS7, GTP, Diameter & SIP.
- [5GC_API_parse](https://github.com/PentHertz/5GC_API_parse) - 5GC API parse is a BurpSuite extension allowing to assess 5G core network functions, by parsing the OpenAPI 3.0 not supported by previous OpenAPI extension in Burp, and generating requests for intrusion tests purposes.
- [FirmWire](https://github.com/FirmWire/FirmWire) - FirmWire is a full-system baseband firmware emulation platform for fuzzing, debugging, and root-cause analysis of smartphone baseband firmwares.

### Videos and papers

- [Exploiting Possible 5G Vulnerabilities](https://blog.3g4g.co.uk/2019/10/exploiting-possible-5g-vulnerabilities.html) a blog post on the 3G/4G blog about the latest HITB talk describing attack in 5G.
- [USENIX19 Hiding in Plain Signal:Physical Signal Overshadowing Attack on LTE](https://www.usenix.org/system/files/sec19-yang-hojoon.pdf) - SigOver - Overriding LTE broadcast message using signal capture effect and good enough time synchronization.
- [HITB talk : 4G LTE Man in the Middle Attack with a Hacked Femtocell](https://gsec.hitb.org/materials/sg2019/D2%20-%204G%20LTE%20Man%20in%20the%20Middle%20Attacks%20with%20a%20Hacked%20Femtocell%20-%20Xiaodong%20Zou.pdf) - high level talk on hacking 4G smallcell, sourcing, tools, opportunities including on S1 gateway.
- [Vulnerabilities in 5G](https://infosec.sintef.no/en/informasjonssikkerhet/2019/08/new-vulnerabilities-in-5g-security-architecture-countermeasures/) New vulnerabilities in 5G Security Architecture & Countermeasures.
- [QPSI-2019-LTEFuzz](https://www.youtube.com/watch?v=1ns46Uy1lM0&feature=youtu.be) - Security analysis of the LTE control plane with LTEFuzz, talk regarded at QPSI Product Security Summit.
- [LTEInspector: A Systematic Approach for Adversarial Testing of 4G LTE](https://www.youtube.com/watch?v=Cf6-O63vVdI) - Talk about LTE vulnerability research at NDSS 2018.
- [SS7: Locate. Track. Manipulate.](https://media.ccc.de/v/31c3_-_6249_-_en_-_saal_1_-_201412271715_-_ss7_locate_track_manipulate_-_tobias_engel) - Talk about SS7 vulnerability at 31C3.
- [SS7map : mapping vulnerability of the international mobile roaming infrastructure](https://media.ccc.de/v/31c3_-_6531_-_en_-_saal_6_-_201412272300_-_ss7map_mapping_vulnerability_of_the_international_mobile_roaming_infrastructure_-_laurent_ghigonis_-_alexandre_de_oliveira) - Talk about SS7 vulnerability and introduction to [SS7map](https://ss7map.p1sec.com/) at 31C3.
- [Advanced interconnect attacks](https://media.ccc.de/v/camp2015-6785-advanced_interconnect_attacks) - Talk about GTP interconnection security at Chaos Communication Camp 2015.
- [Mobile Data Interception from the Interconnection Link](https://media.ccc.de/v/34c3-8879-mobile_data_interception_from_the_interconnection_link) - Talk about Diameter interconnection security at 34C3.
- [On the Challenges of Automata Reconstruction in LTE Networks](https://www.syssec.ruhr-uni-bochum.de/media/emma/veroeffentlichungen/2021/06/02/LTE-Automata-WiSec21.pdf) - In this paper, the authors explore active automata learning for 4G/LTE protocol state machines. [video](https://www.youtube.com/watch?v=0OERPpdeJi8)
- [SS7 and SIGTRAN in 2G/3G networks](https://people.osmocom.org/tnt/osmodevcall/osmodevcall-20210514-laforge-ss7-sigtran_h264_420.mp4) - An introduction to SS7/SIGTRAN stack, including the history, use cases, roles of each layer, and how SS7-speaking equipment works.
- [Hiding in plain signal: Physical signal overshadowing attack on LTE](https://syssec.kaist.ac.kr/pub/2019/sec19-yang-hojoon.pdf) - n this paper, for the first time, we present a signal injection attack that exploits the funda- mental weaknesses of broadcast messages in LTE and mod- ifies a transmitted signal over the air.

### Writeups

- [How the CCC Camp 2019 LTE network works](http://people.osmocom.org/laforge/slides/cccamp2019-how_the_camp_lte_works.pdf) - write up on reusing commercial Ericsson 4G units.
- [GSM capture, analysis and decoding](http://domonkos.tomcsanyi.net/?p=418) - four posts series on GSM cellular signal analysis.

## Blogs
- [Nick vs Networking](https://nickvsnetworking.com/category/plmn/) - So this blog focuses on telecommunications network engineering, from the very old (Shout out to the National Communications Museum), to very new and everything in between.
- [The 3G4G Blog](https://blog.3g4g.co.uk) - Latest news and information on 3G, 4G, 5G wireless and technologies in general.
- [Frédéric Launay - Les réseaux de mobiles 4G et 5G](http://blogs.univ-poitiers.fr/f-launay/) - [FR] Ce blog est un site de vulgarisation sur la téléphonie mobile de 4ème Génération ou 4G, du LTE et du web 2.O.
- [Yoshiyuki Kurauchi](https://wmnsk.com/posts/) - Blog posts by Yoshiyuki Kurauchi - A telecom / networking / security enthusiast.
- [How LTE Stuff Works?](https://howltestuffworks.blogspot.com/) - Blogs on 4G/5G by a 3GPP Engineer.

## Organizations

- [Osmocom](https://osmocom.org) Umbrella for numerous opensource mobile communications projects. Recordings of many great presentations can be found on their [OsmoDevCon](https://osmocom.org/projects/osmo-dev-con/wiki/OsmoDevCon) page (It's held online as [OsmoDevCall](https://osmocom.org/projects/osmo-dev-con/wiki/OsmoDevCall) lately).  They also have a web based [discourse forum](https://discourse.osmocom.org/)
- [Sysmocom](http://shop.sysmocom.de) Store frontend for [sysmocom](https://www.sysmocom.de), company providing product, support and services not only related to Osmocom.
- [Telecom Infra Project](https://www.telecominfraproject.com) - FB initiated project to create an equivalent of the OpenCompute project in the telco space.
- [3GPP Forge](https://forge.3gpp.org/rep/explore) - Forge for the 3GPP organization.

## Docs

- [Wireless frequency bands](http://niviuk.free.fr/) - Come for the frequency calculator, stay for the cellular other resources.
- [ShareTechNote](http://www.sharetechnote.com/) - an impressive repo of knowledge for the cellular telco world.
- [3GPP specs](http://www.3gpp.org/ftp/Specs/html-info/36-series.htm) - 3GPP specs.
- [CNTT](https://cntt-n.github.io/CNTT/) - set of reference specifications for NFVI coming from several telcos (Vodafone, Telstra, Orange mentionned as authors).
- [3gpp.guru](https://3gpp.guru) - look up 3GPP abbreviations
- [speX](https://spex.cor-net.org) - accessible 3GPP specs (PDF, DOC, HTML), [can be self-hosted](https://github.com/CoRfr/spex-3gpp)
- [tool3rd](https://github.com/proj3rd/tool3rd) - Assistant for 3GPP telecommunication development
- [3gpp-citations](https://github.com/martisak/3gpp-citations) - 3GPP Bibtex entry generator
- [3GPP-overall-architecture](https://github.com/nickel0/3GPP-Overall-Architecture) - very detailed, high-res PDF of the overall 3GPP architecture
- [Introduce to 5GC](https://github.com/ianchen0119/Introduce-to-5GC) - 5GC & Cloud Native handbook written in traditaional chinese
- [Getsi](https://getsi.org/) - Easy search engine for 3GPP specs
- [eUICC and eSIM Developer Manual](https://euicc-manual.osmocom.org)

## Slides

- [Kubernetes networking in the telco space](https://wiki.lfnetworking.org/download/attachments/328197/KubernetesNetworkingInTheTelcoSpace-Csatari.pdf?version=1&modificationDate=1522083330000&api=v2)

## Tweets

- [srsLTE 2G CSFB and PCAP fixes](https://twitter.com/LaF0rge/status/1158078169477292032)

## Issues

- [SCTP Kubernetes support](https://github.com/kubernetes/community/pull/2276)
- [SRSENB: Add SIB7 (GERAN neighbor) support](https://github.com/srsLTE/srsLTE/pull/361)

## Mailing-lists

- [OpenBSC](https://lists.osmocom.org/mailman/listinfo/openbsc)
- [OAI-user](http://lists.eurecom.fr/sympa/arc/openair5g-user)
- [OAI-devel](http://lists.eurecom.fr/sympa/arc/openair5g-devel)
- [OAI-corenetwork-user](http://lists.eurecom.fr/sympa/arc/openaircn-user)
- [OAI-corenetwork-devel](http://lists.eurecom.fr/sympa/arc/openaircn-devel)
- [magma-dev](https://groups.google.com/forum/#!forum/magma-dev)
- [magma-announce](https://groups.google.com/forum/#!forum/magma-announce)

## YouTube channels

- [penhertz](https://www.youtube.com/@Penthertz) - Official YT channel of Penthertz to talk about RF Hacking, Software-Defined Radio, and other tips and tricks!.

## Slacks

- [Magma](https://slack.magmacore.org/)

## Discord

- [Open5gs](https://discord.gg/M9ARcyvV)

## Commercial 
- [open-cells](https://open-cells.com): 4G and 5G, full open source can implement any test bed using cellular network
- [sysmocom](https://www.sysmocom.de): sysmocom fills a gap in the telecommunications market for development, products and services.
- [5ber esim](http://esim.5ber.com) - 5ber.eSIM card is a physical SIM card that complies with the GSMA standards that can store up to 15 eSIM profiles at the same time.
- [esim.me](https://esim.me) - physical sim card combined with a proprietary app that enable to load up to 15 eSIM on the physical sim card.

## License

[MIT](LICENSE)
