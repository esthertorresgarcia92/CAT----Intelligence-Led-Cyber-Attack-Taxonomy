<div class="container-fluid">
 <h1>
  System Time Discovery
 </h1>
 <div class="row">
  <div class="col-md-8 description-body">
   <p>
    The system time is set and stored by the Windows Time Service within a domain to maintain time synchronization between systems and services in an enterprise network.
    <span class="scite-citeref-number" data-reference="MSDN System Time" id="scite-ref-1-a">
     <sup>
      <a aria-describedby="qtip-0" data-hasqtip="0" href="https://msdn.microsoft.com/ms724961.aspx" target="_blank">
       [1]
      </a>
     </sup>
    </span>
    <span class="scite-citeref-number" data-reference="Technet Windows Time Service" id="scite-ref-2-a">
     <sup>
      <a aria-describedby="qtip-1" data-hasqtip="1" href="https://technet.microsoft.com/windows-server-docs/identity/ad-ds/get-started/windows-time-service/windows-time-service-tools-and-settings" target="_blank">
       [2]
      </a>
     </sup>
    </span>
   </p>
   <p>
    An adversary may gather the system time and/or time zone from a local or remote system. This information may be gathered in a number of ways, such as with
    <a href="https://attack.mitre.org/software/S0039">
     Net
    </a>
    on Windows by performing
    <code>
     net time \hostname
    </code>
    to gather the system time on a remote system. The victim's time zone may also be inferred from the current system time or gathered by using
    <code>
     w32tm /tz
    </code>
    .
    <span class="scite-citeref-number" data-reference="Technet Windows Time Service" id="scite-ref-2-a">
     <sup>
      <a aria-describedby="qtip-1" data-hasqtip="1" href="https://technet.microsoft.com/windows-server-docs/identity/ad-ds/get-started/windows-time-service/windows-time-service-tools-and-settings" target="_blank">
       [2]
      </a>
     </sup>
    </span>
    The information could be useful for performing other techniques, such as executing a file with a
    <a href="https://attack.mitre.org/techniques/T1053">
     Scheduled Task
    </a>
    <span class="scite-citeref-number" data-reference="RSA EU12 They're Inside" id="scite-ref-3-a">
     <sup>
      <a aria-describedby="qtip-2" data-hasqtip="2" href="https://www.rsaconference.com/writable/presentations/file_upload/ht-209_rivner_schwartz.pdf" target="_blank">
       [3]
      </a>
     </sup>
    </span>
    , or to discover locality information based on time zone to assist in victim targeting.
   </p>
  </div>
  <div class="col-md-4">
   <div class="card">
    <div class="card-body">
     <div class="card-data">
      <span class="h5 card-title">
       ID
      </span>
      : T1124
      <br/>
      <br/>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
       Tactic
      </span>
      : Discovery
      <br/>
      <br/>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
       Platform:
      </span>
      Windows
      <br/>
      <br/>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
       Permissions Required:
      </span>
      User
      <br/>
      <br/>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
       Data Sources:
      </span>
      Process monitoring, Process command-line parameters, API monitoring
      <br/>
      <br/>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
      </span>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
       Version
      </span>
      : 1.0
     </div>
    </div>
   </div>
  </div>
 </div>
 <h2 class="pt-3" id="examples">
  Examples
 </h2>
 <table class="table table-bordered table-light mt-2">
  <thead>
   <tr>
    <th scope="col">
     Name
    </th>
    <th scope="col">
     Description
    </th>
   </tr>
  </thead>
  <tbody class="bg-white">
   <tr>
    <td>
     <a href="https://attack.mitre.org/groups/G0060">
      BRONZE BUTLER
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/groups/G0060">
       BRONZE BUTLER
      </a>
      has used
      <code>
       net time
      </code>
      to check the local time on a target system.
      <span class="scite-citeref-number" data-reference="Secureworks BRONZE BUTLER Oct 2017" id="scite-ref-4-a" onclick="scrollToRef('scite-4')">
       <sup>
        <a aria-describedby="qtip-3" data-hasqtip="3" href="https://www.secureworks.com/research/bronze-butler-targets-japanese-businesses" target="_blank">
         [4]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0237">
      GravityRAT
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0237">
       GravityRAT
      </a>
      can obtain the date and time of a system.
      <span class="scite-citeref-number" data-reference="Talos GravityRAT" id="scite-ref-5-a" onclick="scrollToRef('scite-5')">
       <sup>
        <a aria-describedby="qtip-4" data-hasqtip="4" href="https://blog.talosintelligence.com/2018/04/gravityrat-two-year-evolution-of-apt.html" target="_blank">
         [5]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0260">
      InvisiMole
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0260">
       InvisiMole
      </a>
      gathers the local system time from the victim’s machine.
      <span class="scite-citeref-number" data-reference="ESET InvisiMole June 2018" id="scite-ref-6-a" onclick="scrollToRef('scite-6')">
       <sup>
        <a aria-describedby="qtip-5" data-hasqtip="5" href="https://www.welivesecurity.com/2018/06/07/invisimole-equipped-spyware-undercover/" target="_blank">
         [6]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/groups/G0032">
      Lazarus Group
     </a>
    </td>
    <td>
     <p>
      A Destover-like implant used by
      <a href="https://attack.mitre.org/groups/G0032">
       Lazarus Group
      </a>
      can obtain the current system time and send it to the C2 server.
      <span class="scite-citeref-number" data-reference="McAfee GhostSecret" id="scite-ref-7-a" onclick="scrollToRef('scite-7')">
       <sup>
        <a aria-describedby="qtip-6" data-hasqtip="6" href="https://securingtomorrow.mcafee.com/mcafee-labs/analyzing-operation-ghostsecret-attack-seeks-to-steal-data-worldwide/" target="_blank">
         [7]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0149">
      MoonWind
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0149">
       MoonWind
      </a>
      obtains the victim's current time.
      <span class="scite-citeref-number" data-reference="Palo Alto MoonWind March 2017" id="scite-ref-8-a" onclick="scrollToRef('scite-8')">
       <sup>
        <a aria-describedby="qtip-7" data-hasqtip="7" href="http://researchcenter.paloaltonetworks.com/2017/03/unit42-trochilus-rat-new-moonwind-rat-used-attack-thai-utility-organizations/" target="_blank">
         [8]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0039">
      Net
     </a>
    </td>
    <td>
     <p>
      The
      <code>
       net time
      </code>
      command can be used in
      <a href="https://attack.mitre.org/software/S0039">
       Net
      </a>
      to determine the local or remote system time.
      <span class="scite-citeref-number" data-reference="TechNet Net Time" id="scite-ref-9-a" onclick="scrollToRef('scite-9')">
       <sup>
        <a aria-describedby="qtip-8" data-hasqtip="8" href="https://technet.microsoft.com/bb490716.aspx" target="_blank">
         [9]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0264">
      OopsIE
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0264">
       OopsIE
      </a>
      checks to see if the system is configured with "Daylight" time and checks for a specific region to be set for the timezone.
      <span class="scite-citeref-number" data-reference="Unit 42 OilRig Sept 2018" id="scite-ref-10-a" onclick="scrollToRef('scite-10')">
       <sup>
        <a aria-describedby="qtip-9" data-hasqtip="9" href="https://researchcenter.paloaltonetworks.com/2018/09/unit42-oilrig-targets-middle-eastern-government-adds-evasion-techniques-oopsie/" target="_blank">
         [10]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0139">
      PowerDuke
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0139">
       PowerDuke
      </a>
      has commands to get the time the machine was built, the time, and the time zone.
      <span class="scite-citeref-number" data-reference="Volexity PowerDuke November 2016" id="scite-ref-11-a" onclick="scrollToRef('scite-11')">
       <sup>
        <a aria-describedby="qtip-10" data-hasqtip="10" href="https://www.volexity.com/blog/2016/11/09/powerduke-post-election-spear-phishing-campaigns-targeting-think-tanks-and-ngos/" target="_blank">
         [11]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0238">
      Proxysvc
     </a>
    </td>
    <td>
     <p>
      As part of the data reconnaissance phase,
      <a href="https://attack.mitre.org/software/S0238">
       Proxysvc
      </a>
      grabs the system time to send back to the control server.
      <span class="scite-citeref-number" data-reference="McAfee GhostSecret" id="scite-ref-7-a" onclick="scrollToRef('scite-7')">
       <sup>
        <a aria-describedby="qtip-6" data-hasqtip="6" href="https://securingtomorrow.mcafee.com/mcafee-labs/analyzing-operation-ghostsecret-attack-seeks-to-steal-data-worldwide/" target="_blank">
         [7]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0148">
      RTM
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0148">
       RTM
      </a>
      can obtain the victim time zone.
      <span class="scite-citeref-number" data-reference="ESET RTM Feb 2017" id="scite-ref-12-a" onclick="scrollToRef('scite-12')">
       <sup>
        <a aria-describedby="qtip-11" data-hasqtip="11" href="https://www.welivesecurity.com/wp-content/uploads/2017/02/Read-The-Manual.pdf" target="_blank">
         [12]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0140">
      Shamoon
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0140">
       Shamoon
      </a>
      obtains the system time and will only activate if it is greater than a preset date.
      <span class="scite-citeref-number" data-reference="Palo Alto Shamoon Nov 2016" id="scite-ref-13-a" onclick="scrollToRef('scite-13')">
       <sup>
        <a aria-describedby="qtip-12" data-hasqtip="12" href="http://researchcenter.paloaltonetworks.com/2016/11/unit42-shamoon-2-return-disttrack-wiper/" target="_blank">
         [13]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0098">
      T9000
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0098">
       T9000
      </a>
      gathers and beacons the system time during installation.
      <span class="scite-citeref-number" data-reference="Palo Alto T9000 Feb 2016" id="scite-ref-14-a" onclick="scrollToRef('scite-14')">
       <sup>
        <a aria-describedby="qtip-13" data-hasqtip="13" href="http://researchcenter.paloaltonetworks.com/2016/02/t9000-advanced-modular-backdoor-uses-complex-anti-analysis-techniques/" target="_blank">
         [14]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/groups/G0010">
      Turla
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/groups/G0010">
       Turla
      </a>
      surveys a system upon check-in to discover the system time by using the
      <code>
       net time
      </code>
      command.
      <span class="scite-citeref-number" data-reference="Kaspersky Turla" id="scite-ref-15-a" onclick="scrollToRef('scite-15')">
       <sup>
        <a aria-describedby="qtip-14" data-hasqtip="14" href="https://securelist.com/the-epic-turla-operation/65545/" target="_blank">
         [15]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0275">
      UPPERCUT
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0275">
       UPPERCUT
      </a>
      has the capability to obtain the time zone information and current timestamp of the victim’s machine.
      <span class="scite-citeref-number" data-reference="FireEye APT10 Sept 2018" id="scite-ref-16-a" onclick="scrollToRef('scite-16')">
       <sup>
        <a aria-describedby="qtip-15" data-hasqtip="15" href="https://www.fireeye.com/blog/threat-research/2018/09/apt10-targeting-japanese-corporations-using-updated-ttps.html" target="_blank">
         [16]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
  </tbody>
 </table>
 <h2 class="pt-3" id="mitigation">
  Mitigation
 </h2>
 <p>
  Benign software uses legitimate processes to gather system time. Efforts should be focused on preventing unwanted or unknown code from executing on a system. Some common tools, such as net.exe, may be blocked by policy to prevent common ways of acquiring remote system time.
 </p>
 <p>
  Identify unnecessary system utilities or potentially malicious software that may be used to acquire system time information, and audit and/or block them by using whitelisting
  <span class="scite-citeref-number" data-reference="Beechey 2010" id="scite-ref-17-a">
   <sup>
    <a aria-describedby="qtip-16" data-hasqtip="16" href="http://www.sans.org/reading-room/whitepapers/application/application-whitelisting-panacea-propaganda-33599" target="_blank">
     [17]
    </a>
   </sup>
  </span>
  tools, like AppLocker,
  <span class="scite-citeref-number" data-reference="Windows Commands JPCERT" id="scite-ref-18-a">
   <sup>
    <a aria-describedby="qtip-17" data-hasqtip="17" href="http://blog.jpcert.or.jp/2016/01/windows-commands-abused-by-attackers.html" target="_blank">
     [18]
    </a>
   </sup>
  </span>
  <span class="scite-citeref-number" data-reference="NSA MS AppLocker" id="scite-ref-19-a">
   <sup>
    <a aria-describedby="qtip-18" data-hasqtip="18" href="https://www.iad.gov/iad/library/ia-guidance/tech-briefs/application-whitelisting-using-microsoft-applocker.cfm" target="_blank">
     [19]
    </a>
   </sup>
  </span>
  or Software Restriction Policies
  <span class="scite-citeref-number" data-reference="Corio 2008" id="scite-ref-20-a">
   <sup>
    <a aria-describedby="qtip-19" data-hasqtip="19" href="http://technet.microsoft.com/en-us/magazine/2008.06.srp.aspx" target="_blank">
     [20]
    </a>
   </sup>
  </span>
  where appropriate.
  <span class="scite-citeref-number" data-reference="TechNet Applocker vs SRP" id="scite-ref-21-a">
   <sup>
    <a aria-describedby="qtip-20" data-hasqtip="20" href="https://technet.microsoft.com/en-us/library/ee791851.aspx" target="_blank">
     [21]
    </a>
   </sup>
  </span>
 </p>
 <h2 class="pt-3" id="detection">
  Detection
 </h2>
 <p>
  Command-line interface monitoring may be useful to detect instances of net.exe or other command-line utilities being used to gather system time or time zone. Methods of detecting API use for gathering this information are likely less useful due to how often they may be used by legitimate software.
 </p>
 <h2 class="pt-3" id="references">
  References
 </h2>
 <div class="row">
  <div class="col">
   <ol>
    <li>
     <span class="scite-citation" id="scite-1">
      <span class="scite-citation-text">
       <a class="external text" href="https://msdn.microsoft.com/ms724961.aspx" name="scite-1" rel="nofollow" target="_blank">
        Microsoft. (n.d.). System Time. Retrieved November 25, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-2">
      <span class="scite-citation-text">
       <a class="external text" href="https://technet.microsoft.com/windows-server-docs/identity/ad-ds/get-started/windows-time-service/windows-time-service-tools-and-settings" name="scite-2" rel="nofollow" target="_blank">
        Mathers, B. (2016, September 30). Windows Time Service Tools and Settings. Retrieved November 25, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-3">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.rsaconference.com/writable/presentations/file_upload/ht-209_rivner_schwartz.pdf" name="scite-3" rel="nofollow" target="_blank">
        Rivner, U., Schwartz, E. (2012). They’re Inside… Now What?. Retrieved November 25, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-4">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.secureworks.com/research/bronze-butler-targets-japanese-businesses" name="scite-4" rel="nofollow" target="_blank">
        Counter Threat Unit Research Team. (2017, October 12). BRONZE BUTLER Targets Japanese Enterprises. Retrieved January 4, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-5">
      <span class="scite-citation-text">
       <a class="external text" href="https://blog.talosintelligence.com/2018/04/gravityrat-two-year-evolution-of-apt.html" name="scite-5" rel="nofollow" target="_blank">
        Mercer, W., Rascagneres, P. (2018, April 26). GravityRAT - The Two-Year Evolution Of An APT Targeting India. Retrieved May 16, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-6">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.welivesecurity.com/2018/06/07/invisimole-equipped-spyware-undercover/" name="scite-6" rel="nofollow" target="_blank">
        Hromcová, Z. (2018, June 07). InvisiMole: Surprisingly equipped spyware, undercover since 2013. Retrieved July 10, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-7">
      <span class="scite-citation-text">
       <a class="external text" href="https://securingtomorrow.mcafee.com/mcafee-labs/analyzing-operation-ghostsecret-attack-seeks-to-steal-data-worldwide/" name="scite-7" rel="nofollow" target="_blank">
        Sherstobitoff, R., Malhotra, A. (2018, April 24). Analyzing Operation GhostSecret: Attack Seeks to Steal Data Worldwide. Retrieved May 16, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-8">
      <span class="scite-citation-text">
       <a class="external text" href="http://researchcenter.paloaltonetworks.com/2017/03/unit42-trochilus-rat-new-moonwind-rat-used-attack-thai-utility-organizations/" name="scite-8" rel="nofollow" target="_blank">
        Miller-Osborn, J. and Grunzweig, J.. (2017, March 30). Trochilus and New MoonWind RATs Used In Attack Against Thai Organizations. Retrieved March 30, 2017.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-9">
      <span class="scite-citation-text">
       <a class="external text" href="https://technet.microsoft.com/bb490716.aspx" name="scite-9" rel="nofollow" target="_blank">
        Microsoft. (n.d.). Net time. Retrieved November 25, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-10">
      <span class="scite-citation-text">
       <a class="external text" href="https://researchcenter.paloaltonetworks.com/2018/09/unit42-oilrig-targets-middle-eastern-government-adds-evasion-techniques-oopsie/" name="scite-10" rel="nofollow" target="_blank">
        Falcone, R., et al. (2018, September 04). OilRig Targets a Middle Eastern Government and Adds Evasion Techniques to OopsIE. Retrieved September 24, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-11">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.volexity.com/blog/2016/11/09/powerduke-post-election-spear-phishing-campaigns-targeting-think-tanks-and-ngos/" name="scite-11" rel="nofollow" target="_blank">
        Adair, S.. (2016, November 9). PowerDuke: Widespread Post-Election Spear Phishing Campaigns Targeting Think Tanks and NGOs. Retrieved January 11, 2017.
       </a>
      </span>
     </span>
    </li>
   </ol>
  </div>
  <div class="col">
   <ol start="12.5">
    <li>
     <span class="scite-citation" id="scite-12">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.welivesecurity.com/wp-content/uploads/2017/02/Read-The-Manual.pdf" name="scite-12" rel="nofollow" target="_blank">
        Faou, M. and Boutin, J.. (2017, February). Read The Manual: A Guide to the RTM Banking Trojan. Retrieved March 9, 2017.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-13">
      <span class="scite-citation-text">
       <a class="external text" href="http://researchcenter.paloaltonetworks.com/2016/11/unit42-shamoon-2-return-disttrack-wiper/" name="scite-13" rel="nofollow" target="_blank">
        Falcone, R.. (2016, November 30). Shamoon 2: Return of the Disttrack Wiper. Retrieved January 11, 2017.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-14">
      <span class="scite-citation-text">
       <a class="external text" href="http://researchcenter.paloaltonetworks.com/2016/02/t9000-advanced-modular-backdoor-uses-complex-anti-analysis-techniques/" name="scite-14" rel="nofollow" target="_blank">
        Grunzweig, J. and Miller-Osborn, J.. (2016, February 4). T9000: Advanced Modular Backdoor Uses Complex Anti-Analysis Techniques. Retrieved April 15, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-15">
      <span class="scite-citation-text">
       <a class="external text" href="https://securelist.com/the-epic-turla-operation/65545/" name="scite-15" rel="nofollow" target="_blank">
        Kaspersky Lab's Global Research and Analysis Team. (2014, August 7). The Epic Turla Operation: Solving some of the mysteries of Snake/Uroburos. Retrieved December 11, 2014.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-16">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.fireeye.com/blog/threat-research/2018/09/apt10-targeting-japanese-corporations-using-updated-ttps.html" name="scite-16" rel="nofollow" target="_blank">
        Matsuda, A., Muhammad I. (2018, September 13). APT10 Targeting Japanese Corporations Using Updated TTPs. Retrieved September 17, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-17">
      <span class="scite-citation-text">
       <a class="external text" href="http://www.sans.org/reading-room/whitepapers/application/application-whitelisting-panacea-propaganda-33599" name="scite-17" rel="nofollow" target="_blank">
        Beechey, J. (2010, December). Application Whitelisting: Panacea or Propaganda?. Retrieved November 18, 2014.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-18">
      <span class="scite-citation-text">
       <a class="external text" href="http://blog.jpcert.or.jp/2016/01/windows-commands-abused-by-attackers.html" name="scite-18" rel="nofollow" target="_blank">
        Tomonaga, S. (2016, January 26). Windows Commands Abused by Attackers. Retrieved February 2, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-19">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.iad.gov/iad/library/ia-guidance/tech-briefs/application-whitelisting-using-microsoft-applocker.cfm" name="scite-19" rel="nofollow" target="_blank">
        NSA Information Assurance Directorate. (2014, August). Application Whitelisting Using Microsoft AppLocker. Retrieved March 31, 2016.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-20">
      <span class="scite-citation-text">
       <a class="external text" href="http://technet.microsoft.com/en-us/magazine/2008.06.srp.aspx" name="scite-20" rel="nofollow" target="_blank">
        Corio, C., &amp; Sayana, D. P. (2008, June). Application Lockdown with Software Restriction Policies. Retrieved November 18, 2014.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-21">
      <span class="scite-citation-text">
       <a class="external text" href="https://technet.microsoft.com/en-us/library/ee791851.aspx" name="scite-21" rel="nofollow" target="_blank">
        Microsoft. (2012, June 27). Using Software Restriction Policies and AppLocker Policies. Retrieved April 7, 2016.
       </a>
      </span>
     </span>
    </li>
   </ol>
  </div>
 </div>
</div>
