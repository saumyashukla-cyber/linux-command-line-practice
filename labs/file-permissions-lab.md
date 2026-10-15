*Linux File Permissions Lab*

Objective
Understand Linux file permissions and practise changing permissions using chmod.

Environment
- Operating System: Kali Linux

Commands Practised

1. Create a test file
```bash
touch testfile.txt
```

2. View file permissions
```bash
ls -l testfile.txt
```

3. Set permissions to 755
```bash
chmod 755 testfile.txt
ls -l testfile.txt
```

4. Set permissions to 640
```bash
chmod 640 testfile.txt
ls -l testfile.txt
```

Learning Outcomes
- Learned how to inspect file permissions.
- Practised modifying permissions with chmod.
- Understood the difference between owner, group, and other permissions.

Security Relevance
Appropriate file permissions help prevent unauthorized users from reading or modifying files.

## Result
Commands were documented for practice in a personal Linux lab.
