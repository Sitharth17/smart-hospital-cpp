# Smart Hospital — Fresh C++ Version

This is a standalone C++ web project. It does NOT depend on the old Node.js project.

## VS Code / Windows
Install MinGW-w64 (g++), open this folder in VS Code, then:

```powershell
g++ -std=c++17 -O2 -pthread main.cpp -o hospital.exe
.\hospital.exe
```

Open `http://localhost:3000`.

## Render
The included `Dockerfile` and `render.yaml` are ready for a Render Web Service. Push the folder to GitHub and create a Web Service from that repository. Render builds the C++ server and passes its `PORT` automatically.

## Staff login
- admin / Admin@123
- reception / Reception@123
- sitharth / Sith@123
- jenifar / Jeni@456
- berline / bella@789
- puvanesh / Puvan@321
- hari / Hari@654

Patients can create an account from the login page. Reception can link that username when registering a visit; only then does that account see its visit/token.

## Included
Patient self-registration, reception visit registration, token generation, priority queue, doctor-specific access, patient-only own records, consultation notes, completion, appointments, doctor departments, analytics, admin audit log, password change, and simple file persistence.

Educational prototype only. Do not enter real patient/medical data. The included demo credentials and simple built-in HTTP/session/password approach are for a college prototype, not production healthcare use.
