# Enumeration

## 

## Windows Privilege Escalation

### Services

Are there any services that you have the ability to start and stop?

Are there any Unquoted Service Path directories you can write to?

* Use `sc qc <service name>` to enumerate.
* Check if you can START and STOP the service
* If you can't START/STOP, check if it AUTO\_STARTS
  * If it AUTO\_STARTS, can you reboot?

### Web Applications

* What is the version?
  * Look everywhere
* Search for exploits not only on Searchsploit, but other places, because Searchsploit isn't always a 1:1 updated version of exploit-db \(Jacko on PG\).
  * Exploit-db
  * Google \| Git

### Overcoming Shell Limitations

* Are we in constrained language mode?
  * Constrained language mode locks down features of Powershell that are usually required for complex attacks. **Reading Material**
    * [Powershell Constrained Language Mode](https://devblogs.microsoft.com/powershell/powershell-constrained-language-mode/) - Great Explanation
    * [Bypassing Constrained Language Mode](https://www.ired.team/offensive-security/code-execution/powershell-constrained-language-mode-bypass)
  * To check for constrained language mode: `powershell ExecutionContext.SessionState.LanguageMode`



