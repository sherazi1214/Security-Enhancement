# Security-Enhancement

## 1. **[Enhancing Security](https://github.com/sherazi1214/Enhancing-Security/blob/main/README.md)**

## 2.  **[TCP/IP Transmission Control Protocol](https://github.com/sherazi1214/TCP-IP-Transmission-Control-Protocol)**

## 3. **[Email-Security](https://github.com/sherazi1214/Email-Security-/blob/main/README.md)**


## 4. Group Policy (Windows)

**English:**
Group Policy is a Windows feature used to centrally manage and configure operating systems, applications, and user settings in an Active Directory (AD) environment.

It allows administrators to enforce security, restrictions, and configurations on multiple computers.

**Urdu:**
Yani ek central control system jahan se admin poori organization ke computers ka behavior control kar sakta hai.

## Group Policy Object (GPO)

English:
A GPO is a collection of policy settings. It can apply to users or computers.

**Examples:** Disable USB ports, enforce password complexity, restrict control panel access, apply firewall rules.

GPOs are linked to Active Directory containers (sites, domains, or OUs).

**Urdu:**

**GPO =** rules ka package jo apply hota hai users/computers par.

## OU (Organizational Unit)

**English:**

OU is an Active Directory container where users, groups, and computers are placed.

GPOs can be applied to OUs for more granular control.

Example: Different policies for HR OU vs IT OU.

**Urdu:**
OU ek folder jaisa hota hai AD ke andar, jahan specific users/computers group kiye jate hain policies ke liye.

## GPMC (Group Policy Management Console)

**English:**

GPMC is the management tool in Windows used to create, edit, link, and manage GPOs.

**Features:** Group Policy Modeling, Resultant Set of Policy (RSoP) reports, linking GPOs to OUs.

**Urdu:**
Ye ek central console hai jahan admin sari policies design aur apply karta hai.

## Group Policy for Security Enhancement (Windows)

**English:**
Admins use GPOs to enforce security best practices:

Password policies (complexity, expiration).

Account lockout thresholds.

Restrict USB access.

Firewall configuration.

Software restrictions / AppLocker.

Deploy security patches.

Audit policies (logging user activity).

**Urdu:**
GPOs ka main kaam hota hai system ko secure aur compliant banana.

## Security Enhancement in Linux

**English:**
Linux doesn’t use GPO but has other mechanisms:

**PAM (Pluggable Authentication Modules):** for authentication policies.

**iptables/firewalld:** for firewall rules.

**Auditd:** for logging and auditing.

**AppArmor / SELinux:** for mandatory access control (MAC).

**Urdu:**
Windows me GPO hota hai, Linux me modules aur policies use hote hain.

## SELinux (Security-Enhanced Linux)

**English:**
SELinux is a Linux security module that enforces Mandatory Access Control (MAC) policies beyond standard file permissions.

Developed by NSA and integrated into Red Hat, CentOS, Fedora.

Ensures processes only access resources they are explicitly allowed to.

**Urdu:**
SELinux ek strict security guard hai jo decide karta hai ke kaunsa process kis file/resource ko access kar sakta hai.

## SELinux Role-Based Access Control (RBAC)

**English:**
SELinux implements RBAC by assigning roles to processes and users:

**Types:** Defines access rules for subjects (processes) and objects (files).

**Roles:** Group of rules given to a user/process.

**Domains:** Execution environment for a process.

**Policy:** Mapping between roles, domains, and types.

**Example:**

Web server process (httpd_t) can only read web files (/var/www/html) but cannot read /etc/shadow.

Database process (mysqld_t) can only access database directories.

**Urdu:**
RBAC me roles assign kiye jate hain, aur har role sirf apni limited cheezon ko access kar sakta hai.

##Summary 

**Group Policy** = Windows ka central control.

**GPO** = rule set.

**OU** = AD folder for users/computers.

**GPMC** = policy management console.

**Windows Security GPO** = enforce password, firewall, restrictions.

**Linux Security** = PAM, iptables, Auditd, SELinux.

**SELinux RBAC** = strict role-based access → process only allowed kaam karega.
