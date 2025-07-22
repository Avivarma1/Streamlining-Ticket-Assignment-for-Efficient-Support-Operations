# Streamlining Ticket Assignment for Efficient Support Operations

This repository contains a ServiceNow update set (`.xml` format) developed to automate and streamline the assignment of support tickets in a ServiceNow environment. The customization is built on the **Global** scope and includes enhancements to ACLs, dictionary entries, table definitions, roles, and a Flow Designer flow.

## 🛠️ Features

- **Custom Table**: `Operations related (u_operations_related)` to track ticket operations.
- **Fields**:
  - `Assigned to user` (Reference field to `sys_user`)
  - `Priority` (String)
- **Roles**:
  - Custom role `u_operations_related_user` to manage access.
- **Access Controls**:
  - Field-level and record-level ACLs for secure data access.
- **Flow Designer Flow**:
  - Triggered on record insert/update based on `u_issue` field conditions.
  - Automates actions like notifications or assignments.

## 📦 File Structure

- `sys_remote_update_set_aa878a87c3fa26109d92b6fdd401317d.xml`: The ServiceNow update set containing all configuration changes.

## 🚀 How to Use

1. **Login to your ServiceNow instance**.
2. **Navigate to System Update Sets → Retrieved Update Sets**.
3. **Import the XML file** from this repository.
4. **Preview and commit** the update set.
5. **Verify** the table `Operations related` and its related configurations.

## 🔐 Requirements

- A valid ServiceNow admin account.
- Access to update sets and Flow Designer.
- The instance must be in a version compatible with Flow Designer.

## 👤 Author

**Admin** – July 22, 2025  
For customization and integration support, feel free to contact or fork the project.

## 📄 License

This project is for educational or internal use. Please follow your organization’s guidelines for importing update sets into a production environment.
