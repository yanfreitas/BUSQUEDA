# BUSQUEDA

![image](https://github.com/yanfreitas/BUSQUEDA/assets/57323947/f08d2c25-73f3-4bd5-8b18-ff5a4021ef55)

Busqueda is an Easy Difficulty Linux machine that involves exploiting a command injection vulnerability present in a `Python` module. By leveraging this vulnerability, we gain user-level access to the machine. To escalate privileges to `root`, we discover credentials within a `Git` config file, allowing us to log into a local `Gitea` service. Additionally, we uncover that a system checkup script can be executed with `root` privileges by a specific user. By utilizing this script, we enumerate `Docker` containers that reveal credentials for the `administrator` user&amp;amp;#039;s `Gitea` account. Further analysis of the system checkup script&amp;amp;#039;s source code in a `Git` repository reveals a means to exploit a relative path reference, granting us Remote Code Execution (RCE) with `root` privileges.
