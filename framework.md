# Aslan Framework Documentation

## 1. Problem Statement

### Core Problem
Relapse in mental health and addiction recovery is a critical issue. Many individuals relapse because they lack immediate, accessible tools to process their emotions, identify their needs, and act in alignment with their values during moments of crisis.

### Importance

#### Personal Impact
- Loss of self-esteem
- Health risks
- Setbacks in recovery progress
- Disruption of personal relationships
- Potential loss of employment or educational opportunities

#### Societal Impact
- Increased healthcare costs
- Strain on support systems
- Impact on community resources
- Burden on emergency services
- Ripple effects on families and support networks

#### Financial Impact
- Healthcare provider costs
- Family financial burden
- Community resource allocation
- Lost productivity
- Treatment program expenses

### Gap in Current Solutions
Traditional support mechanisms (therapy, support groups) often have limitations:
- Lack of 24/7 accessibility
- Geographic constraints
- Cost barriers
- Delayed response times
- Limited personalization

## 2. Solution Overview

### What is Aslan?
Aslan is an innovative AI-driven emotional support system designed to complement traditional therapeutic approaches. It functions as a personal, real-time assistant to help users navigate emotional crises and prevent relapse.

## 3. Technical Architecture

### Database Schema

#### User Management (aslan_users)
- Secure user authentication and profile management
- Fields:
  - Employee ID tracking
  - Username and email for identification
  - Secure password storage
  - Birthday for age-appropriate support
  - Audit timestamps (created, updated, deleted)

#### Chat Session Management (aslan_chat_sessions)
- Tracks individual support sessions
- Fields:
  - User association
  - Session duration tracking (start/end times)
  - Token consumption monitoring
  - Audit timestamps

#### Conversation History (aslan_chat_history)
- Detailed message tracking with emotional analysis
- Fields:
  - Session and user association
  - Message content
  - Message type (user/AI)
  - Emotion labeling (angry, sad, calm, etc.)
  - Color-coded severity flags (red, yellow, green)
  - Audit timestamps

#### Token Usage Monitoring (aslan_user_token_usage)
- Resource allocation and usage tracking
- Fields:
  - User association
  - Monthly token allocation
  - Usage tracking
  - Billing period tracking (start/end dates)

#### Alert System (aslan_alerts)
- Crisis detection and intervention
- Fields:
  - Session and message association
  - Alert classification
  - Severity description
  - Resolution tracking
  - Timestamp tracking

#### Reward System (aslan_rewards)
- Engagement and progress incentivization
- Fields:
  - User association
  - Reward classification
  - Achievement description
  - Grant timing

### Core Features Implementation

#### 1. Real-time Support System
- 24/7 chat availability through aslan_chat_sessions
- Immediate response capability
- Session-based interaction tracking
- Token usage monitoring for resource management

#### 2. Emotional Intelligence
- Message-level emotion tracking
- Color-coded severity assessment
- Pattern recognition through chat history
- Contextual response generation

#### 3. Crisis Management
- Automated alert generation
- Severity-based intervention
- Resolution tracking
- Emergency protocol activation

#### 4. Progress Tracking
- Token usage monitoring
- Session history analysis
- Reward system integration
- Engagement metrics

#### 5. Security and Privacy
- Secure user authentication
- Data encryption
- Audit trail maintenance
- Soft deletion support

### Integration Points

#### Frontend Integration
- Real-time WebSocket communication
- Emotion visualization
- Token usage display
- Alert notifications
- Reward presentations

#### Backend Services
- Authentication service
- Chat processing engine
- Emotion analysis system
- Token management service
- Alert processing system

### Scalability Considerations
- Session management optimization
- Token usage monitoring
- Message history archival
- Alert processing prioritization
- Reward system extensibility

## 4. Future Enhancements
- Advanced emotion detection algorithms
- Enhanced crisis prediction
- Expanded reward mechanisms
- Integration with external support services
- Advanced analytics and reporting

This framework serves as a living document and will evolve with the platform's development and user needs.
