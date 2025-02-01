# EyeNet System Architecture Notes

## Technical Background

### NetFlow Integration
- Cisco NetFlow is the primary flow-based network monitoring tool
- NetFlow probes attach to switches as special modules
- Supports UDP (User Datagram Protocol) and SCTP (Stream Control Transmission Protocol)
- Enables network flow record generation and export

### PayLess SDN Framework
- Provides RESTful API for flow statistics
- Implements adaptive statistics collection
- Delivers real-time information with minimal overhead
- Supports multiple aggregation levels

### Network Architecture
1. **Data Plane**
   - Handles network device management
   - Responsible for efficient data forwarding
   - Includes physical networking devices

2. **Control Plane**
   - Manages forwarding protocols
   - Populates forwarding tables
   - Enforces network policies

3. **Management Plane**
   - Handles remote monitoring
   - Configures control functionality
   - Defines network policies

## System Overview
EyeNet is a Software-Defined Network (SDN) for Decision Support with Descriptive Analytics, designed to provide comprehensive network monitoring and management capabilities.

## Architecture Components

### 1. User Roles
- **Network Administrator**
  - Full system access
  - Can manage IPs, passwords, and restrictions
  - Generate and view all reports
  - Monitor network usage
  
- **Department Staff**
  - Limited access to network information
  - Can view assigned reports
  - Access to usage statistics

### 2. Core Functionalities

#### 2.1 IP Management (Level 2 DFD)
- Add IP address (1.1)
- Assign Department (1.2)
- Select IP address (1.3)
- Monitor Usage (1.4)

#### 2.2 Password Management (Level 2 DFD)
- Enter password (2.1)
- Change password (2.2)
- Secure password update flow

#### 2.3 Network Usage Monitoring (Level 2 DFD)
- Select IP address (3.1)
- View Network Usage (3.2)
- View most visited website (3.3)

#### 2.4 Analytics System (Level 2 DFD)
- IP-based internet usage tracking
- Most visited website analysis
- Department usage statistics
- Traffic analysis reports

### 3. System Architecture Layers

#### Application Layer
- Decision Support System
- Social Media Integration
  - YouTube
  - Instagram
  - Facebook
  - Twitter
  - Google+

#### Monitoring Plane
- Network Monitoring
- OpenFlow Integration
- Northbound API Interface

#### Data Plane
- Hardware Management
  - Wireless Access Points
  - Switches
  - Routers
  - Servers
- Southbound API Interface

### 4. Interface Features

#### Dashboard Components
- Network Traffic Visualization
  - IN/OUT traffic monitoring
  - 1-min average calculations
  - Traffic statistics (Total, Max, Min, Average)
- Connected Devices Monitoring
  - IP Address tracking
  - Latency measurements
  - MAC address logging
  - Manufacturer identification

#### Analytics Interface
- Traffic Activity Visualization
- IP-based monitoring
- Top App Performance tracking
- Bandwidth utilization metrics
- Network usage patterns

### 5. Key Metrics Tracked
- Network Traffic (IN/OUT)
- Bandwidth Utilization
- Device Latency
- User Activity Patterns
- Department Usage Statistics
- Website Access Patterns

### 6. Security Features
- Password Protection
- Access Level Control
- Network Restrictions
- Usage Monitoring
- Analytics-based Threat Detection

## Project Scope

### Target Environment
- College building with 24 offices (UPHSL)
- Server-based monitoring system
- OpenFlow system implementation
- Descriptive analytics focus

### Reporting Schedule
- Daily summaries
- Weekly analysis
- Monthly trends

### Limitations
- No direct bandwidth control
- Manual troubleshooting required
- Focus on monitoring rather than control

## Integration Requirements
1. OpenFlow Protocol Support
2. API Integration (Northbound/Southbound)
3. Database Management System
4. Real-time Monitoring System
5. Analytics Processing Engine

## Reporting Capabilities
1. IP Report
2. Performance Report
3. Network Usage Report
4. Analytics Report
5. Department Usage Statistics
6. Most Visited Websites
7. Traffic Pattern Analysis

---
Note: This documentation will be updated as more system details become available.
