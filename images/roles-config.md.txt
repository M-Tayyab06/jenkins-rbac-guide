# 🔐 Jenkins Role Configuration (Permission Matrix)

Below is an example configuration for roles created in Jenkins using the Role Strategy Plugin.

---

## 🛠️ Role: admin

| Category   | Permissions           |
|------------|------------------------|
| Overall    | Administer, Read       |
| Credentials| All (View, Create, Delete, Update) |
| Agent      | All                    |
| Job        | All                    |
| Run        | All                    |
| View       | All                    |
| SCM        | Read, Tag              |
| Metrics    | All                    |

---

## 👁️ Role: viewer

| Category   | Permissions           |
|------------|------------------------|
| Overall    | Read                   |
| Job        | Read, Workspace        |
| View       | Read                   |
| Metrics    | View, HealthCheck      |

---

## 📎 Notes

- Roles can be fine-tuned based on job or agent-based views
- Permissions can be scoped to folders using **Folder-Based Authorization Strategy**
- Jenkins also supports scripting for automation via Groovy

