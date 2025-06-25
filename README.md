# Catch Me If You Can - Game Database

## Overview
This database system is designed for "Catch Me If You Can", a multiplayer social deduction game similar to Among Us. The database manages all aspects of the game including players, games, maps, tasks, clans, administration, and reporting systems.

## 🎮 Game Features

### Core Gameplay
- **Multiplayer Social Deduction**: Players take on roles as impostors, crewmates, medics, or engineers
- **Map-Based Gameplay**: Multiple maps with unique tasks and environments
- **Task System**: Players complete various tasks while trying to identify impostors
- **Real-time Game Sessions**: Live lobbies with multiple players

### Player System
- **User Profiles**: Complete player profiles with statistics and progression
- **Leveling System**: XP-based progression with unlockable content
- **Win/Loss Tracking**: Comprehensive statistics tracking
- **Regional Support**: Player organization by geographic regions
- **Inventory System**: Collectible items including hats, skins, and pets

### Social Features
- **Clan System**: Players can create and join clans with hierarchical roles
- **Clan-based Games**: Special clan lobbies and competitions
- **Player Reporting**: Community-driven moderation system
- **Social Statistics**: Clan performance tracking and member management

### Administrative Features
- **Multi-level Admin System**: Superadmins, moderators, and analysts
- **Player Moderation**: Ban and mute system with duration controls
- **Admin Action Logging**: Complete audit trail of administrative actions
- **Report Management**: Tools for reviewing and resolving player reports

## 🗄️ Database Structure

### Core Tables

#### Player Management
- **Players**: User profiles, statistics, and progression data
- **Inventory**: Player-owned items and equipment status
- **Items**: Cosmetic items (hats, skins, pets) with unlock requirements

#### Game System
- **Maps**: Game environments organized by categories
- **MapCategories**: Hierarchical organization of maps (Standard, Event, Competitive)
- **Tasks**: Map-specific objectives for players to complete
- **Lobbies**: Game session management with player limits and status
- **Games**: Individual game instances with timing and results
- **GamePlayers**: Player participation in games with roles and outcomes
- **PlayerTasks**: Task assignment and completion tracking

#### Social Features
- **Clans**: Player organizations with leadership structure
- **ClanMembers**: Membership tracking with roles and join dates

#### Administration
- **Admins**: Administrative user accounts with role-based permissions
- **Reports**: Player-submitted reports for misconduct
- **PlayerBans**: Disciplinary actions with duration and reason tracking
- **AdminActions**: Comprehensive logging of all administrative activities

## 🔧 Database Features

### Data Integrity
- **Foreign Key Constraints**: Ensures referential integrity across all relationships
- **Check Constraints**: Validates data values (roles, statuses, item types)
- **Primary Key Constraints**: Guarantees unique identification for all entities
- **Unique Constraints**: Prevents duplicate usernames and clan names

### Performance Optimization
- **Indexed Primary Keys**: Fast lookups for all main entities
- **Composite Keys**: Efficient many-to-many relationship handling
- **Query Optimization**: Designed for common gameplay queries

### Scalability Features
- **Hierarchical Categories**: Flexible map organization system
- **Role-based Access**: Expandable admin permission system
- **Modular Design**: Easy addition of new game features

## 📊 Query Capabilities

The database supports a wide range of analytical and operational queries:

### Player Analytics
- Player profile and statistics retrieval
- Inventory and equipment management
- Regional player distribution analysis
- Level progression tracking
- Win rate calculations

### Game Analytics
- Most difficult tasks identification (failure rate analysis)
- Game session tracking and history
- Map popularity and usage statistics
- Player performance in different roles
- Game duration and completion analytics

### Social Analytics
- Clan membership and activity tracking
- Clan performance comparisons
- Player interaction patterns
- Community growth metrics

### Administrative Queries
- Player moderation history
- Report management and resolution
- Admin activity auditing
- Ban and restriction tracking
- Age-based player analytics

## 🏗️ Implementation Details

### Database Schema Design
- **Third Normal Form (3NF)** compliance to minimize redundancy
- **Entity-Relationship Model** with clear relationships and cardinalities
- **Hierarchical Structures** for categories and clan roles
- **Temporal Data** handling for game sessions and administrative actions

### Security Features
- **Password Hashing** for admin accounts
- **Role-based Access Control** for administrative functions
- **Audit Trail** for all administrative actions
- **Data Validation** through check constraints

### Data Types and Constraints
- **VARCHAR** fields with appropriate length limits
- **TIMESTAMP** fields for precise temporal tracking
- **BOOLEAN** flags for status management
- **INT** fields for numeric identifiers and counters
- **TEXT** fields for detailed descriptions and reasons

## 📁 Project Files

- **`DDL script.txt`**: Complete database schema definition with all tables and constraints
- **`insert_queries.txt`**: Sample data insertion scripts for testing and development
- **`DatebaseQueries.txt`**: Comprehensive collection of operational and analytical queries
- **`ERD, Relational Schema and normalization.pdf`**: Visual database design documentation

## 🚀 Getting Started

1. **Database Setup**: Execute the DDL script to create the database schema
2. **Sample Data**: Run the insert queries to populate the database with test data
3. **Query Testing**: Use the provided queries to verify database functionality
4. **Documentation Review**: Refer to the PDF for visual schema representation

## 🎯 Use Cases

This database system supports:
- **Real-time Multiplayer Gaming**: Live game session management
- **Player Progression Systems**: XP, leveling, and unlockables
- **Community Management**: Clans, reports, and social features
- **Administrative Tools**: Moderation, analytics, and user management
- **Analytics and Reporting**: Player behavior and game performance analysis

## 🔮 Future Enhancements

The database design allows for easy expansion to include:
- Tournament and competitive play systems
- Enhanced social features (friends, messaging)
- Advanced analytics and machine learning integration
- Mobile platform support
- Real-time communication features

---

*This database was designed to provide a robust foundation for a modern multiplayer social deduction game with comprehensive player management, social features, and administrative capabilities.*
