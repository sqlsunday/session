# session
A script that displays currently active sessions along with server and session information

This script shows current status and activity for currently running tasks on
the SQL Server. It returns 6 recordsets, in the following order:

1. General server-wide information
2. Database files, usage, disk space
3. Connections by SPID including CPU and I/O totals
4. Running queries, memory use/grant, query plan
5. Open transactions, type, isolation level
6. Locks by object, partition, including size, wait type, blocking info.

Copyright Daniel Hutmacher under Creative Commons 4.0 license with attribution.
http://creativecommons.org/licenses/by/4.0/

Source:  http://sqlsunday.com/downloads/

**DISCLAIMER:** This script does not make any modifications to the server, except
            for creating three temporary functions in tempdb, used to format
	    values in a user-friendly manner. However, the script may not be
	    suitable to run in a production environment. I cannot assume any
	    responsibility regarding the accuracy of the output information,
	    performance impacts on your server, or any other consequence. If
	    your juristiction does not allow for this kind of waiver/disclaimer,
	    or if you do not accept these terms, you are NOT allowed to store,
	    distribute or use this code in any way.
