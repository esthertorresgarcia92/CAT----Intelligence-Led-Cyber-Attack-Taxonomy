<div class="container-fluid">
 <h1>
  Supply Chain Compromise
 </h1>
 <div class="row">
  <div class="col-md-8 description-body">
   <p>
    Supply chain compromise is the manipulation of products or product delivery mechanisms prior to receipt by a final consumer for the purpose of data or system compromise. Supply chain compromise can take place at any stage of the supply chain including:
   </p>
   <ul>
    <li>
     Manipulation of development tools
    </li>
    <li>
     Manipulation of a development environment
    </li>
    <li>
     Manipulation of source code repositories (public or private)
    </li>
    <li>
     Manipulation of software update/distribution mechanisms
    </li>
    <li>
     Compromised/infected system images (multiple cases of removable media infected at the factory)
    </li>
    <li>
     Replacement of legitimate software with modified versions
    </li>
    <li>
     Sales of modified/counterfeit products to legitimate distributors
    </li>
    <li>
     Shipment interdiction
    </li>
   </ul>
   <p>
    While supply chain compromise can impact any component of hardware or software, attackers looking to gain execution have often focused on malicious additions to legitimate software in software distribution or update channels.
    <span class="scite-citeref-number" data-reference="Avast CCleaner3 2018" id="scite-ref-1-a">
     <sup>
      <a aria-describedby="qtip-0" data-hasqtip="0" href="https://blog.avast.com/new-investigations-in-ccleaner-incident-point-to-a-possible-third-stage-that-had-keylogger-capacities" target="_blank">
       [1]
      </a>
     </sup>
    </span>
    <span class="scite-citeref-number" data-reference="Microsoft Dofoil 2018" id="scite-ref-2-a">
     <sup>
      <a aria-describedby="qtip-1" data-hasqtip="1" href="https://cloudblogs.microsoft.com/microsoftsecure/2018/03/07/behavior-monitoring-combined-with-machine-learning-spoils-a-massive-dofoil-coin-mining-campaign/" target="_blank">
       [2]
      </a>
     </sup>
    </span>
    <span class="scite-citeref-number" data-reference="Command Five SK 2011" id="scite-ref-3-a">
     <sup>
      <a aria-describedby="qtip-2" data-hasqtip="2" href="https://www.commandfive.com/papers/C5_APT_SKHack.pdf" target="_blank">
       [3]
      </a>
     </sup>
    </span>
    Targeting may be specific to a desired victim set
    <span class="scite-citeref-number" data-reference="Symantec Elderwood Sept 2012" id="scite-ref-4-a">
     <sup>
      <a aria-describedby="qtip-3" data-hasqtip="3" href="http://www.symantec.com/content/en/us/enterprise/media/security_response/whitepapers/the-elderwood-project.pdf" target="_blank">
       [4]
      </a>
     </sup>
    </span>
    or malicious software may be distributed to a broad set of consumers but only move on to additional tactics  on specific victims.
    <span class="scite-citeref-number" data-reference="Avast CCleaner3 2018" id="scite-ref-1-a">
     <sup>
      <a aria-describedby="qtip-0" data-hasqtip="0" href="https://blog.avast.com/new-investigations-in-ccleaner-incident-point-to-a-possible-third-stage-that-had-keylogger-capacities" target="_blank">
       [1]
      </a>
     </sup>
    </span>
    <span class="scite-citeref-number" data-reference="Command Five SK 2011" id="scite-ref-3-a">
     <sup>
      <a aria-describedby="qtip-2" data-hasqtip="2" href="https://www.commandfive.com/papers/C5_APT_SKHack.pdf" target="_blank">
       [3]
      </a>
     </sup>
    </span>
   </p>
  </div>
  <div class="col-md-4">
   <div class="card">
    <div class="card-body">
     <div class="card-data">
      <span class="h5 card-title">
       ID
      </span>
      : T1195
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
      : Initial Access
      <br/>
      <br/>
     </div>
     <div class="card-data">
      <span class="h5 card-title">
       Platform:
      </span>
      Linux, Windows, macOS
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
       Data Sources:
      </span>
      Web proxy, File monitoring
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
       CAPEC ID:
      </span>
      <a href="https://capec.mitre.org/data/definitions/437.html" target="_blank">
       CAPEC-437
      </a>
      ,
      <a href="https://capec.mitre.org/data/definitions/438.html" target="_blank">
       CAPEC-438
      </a>
      ,
      <a href="https://capec.mitre.org/data/definitions/439.html" target="_blank">
       CAPEC-439
      </a>
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
     <a href="https://attack.mitre.org/software/S0222">
      CCBkdr
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0222">
       CCBkdr
      </a>
      was added to a legitimate, signed version 5.33 of the CCleaner software and distributed on CCleaner's distribution site.
      <span class="scite-citeref-number" data-reference="Talos CCleanup 2017" id="scite-ref-5-a" onclick="scrollToRef('scite-5')">
       <sup>
        <a aria-describedby="qtip-4" data-hasqtip="4" href="http://blog.talosintelligence.com/2017/09/avast-distributes-malware.html" target="_blank">
         [5]
        </a>
       </sup>
      </span>
      <span class="scite-citeref-number" data-reference="Intezer Aurora Sept 2017" id="scite-ref-6-a" onclick="scrollToRef('scite-6')">
       <sup>
        <a aria-describedby="qtip-5" data-hasqtip="5" href="http://www.intezer.com/evidence-aurora-operation-still-active-supply-chain-attack-through-ccleaner/" target="_blank">
         [6]
        </a>
       </sup>
      </span>
      <span class="scite-citeref-number" data-reference="Avast CCleaner3 2018" id="scite-ref-1-a" onclick="scrollToRef('scite-1')">
       <sup>
        <a aria-describedby="qtip-0" data-hasqtip="0" href="https://blog.avast.com/new-investigations-in-ccleaner-incident-point-to-a-possible-third-stage-that-had-keylogger-capacities" target="_blank">
         [1]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/groups/G0066">
      Elderwood
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/groups/G0066">
       Elderwood
      </a>
      has targeted manufacturers in the supply chain for the defense industry.
      <span class="scite-citeref-number" data-reference="Symantec Elderwood Sept 2012" id="scite-ref-4-a" onclick="scrollToRef('scite-4')">
       <sup>
        <a aria-describedby="qtip-3" data-hasqtip="3" href="http://www.symantec.com/content/en/us/enterprise/media/security_response/whitepapers/the-elderwood-project.pdf" target="_blank">
         [4]
        </a>
       </sup>
      </span>
     </p>
    </td>
   </tr>
   <tr>
    <td>
     <a href="https://attack.mitre.org/software/S0226">
      Smoke Loader
     </a>
    </td>
    <td>
     <p>
      <a href="https://attack.mitre.org/software/S0226">
       Smoke Loader
      </a>
      was distributed through a compromised update to a Tor client with a coin miner payload.
      <span class="scite-citeref-number" data-reference="Microsoft Dofoil 2018" id="scite-ref-2-a" onclick="scrollToRef('scite-2')">
       <sup>
        <a aria-describedby="qtip-1" data-hasqtip="1" href="https://cloudblogs.microsoft.com/microsoftsecure/2018/03/07/behavior-monitoring-combined-with-machine-learning-spoils-a-massive-dofoil-coin-mining-campaign/" target="_blank">
         [2]
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
  Apply supply chain risk management (SCRM) practices and procedures
  <span class="scite-citeref-number" data-reference="MITRE SE Guide 2014" id="scite-ref-7-a">
   <sup>
    <a aria-describedby="qtip-6" data-hasqtip="6" href="https://www.mitre.org/sites/default/files/publications/se-guide-book-interactive.pdf" target="_blank">
     [7]
    </a>
   </sup>
  </span>
  , such as supply chain analysis and appropriate risk management, throughout the life-cycle of a system.
 </p>
 <p>
  Leverage established software development lifecycle (SDLC) practices
  <span class="scite-citeref-number" data-reference="NIST Supply Chain 2012" id="scite-ref-8-a">
   <sup>
    <a aria-describedby="qtip-7" data-hasqtip="7" href="http://dx.doi.org/10.6028/NIST.IR.7622" target="_blank">
     [8]
    </a>
   </sup>
  </span>
  :
 </p>
 <ul>
  <li>
   Uniquely Identify Supply Chain Elements, Processes, and Actors
  </li>
  <li>
   Limit Access and Exposure within the Supply Chain
  </li>
  <li>
   Establish and Maintain the Provenance of Elements, Processes, Tools, and Data
  </li>
  <li>
   Share Information within Strict Limits
  </li>
  <li>
   Perform SCRM Awareness and Training
  </li>
  <li>
   Use Defensive Design for Systems, Elements, and Processes
  </li>
  <li>
   Perform Continuous Integrator Review
  </li>
  <li>
   Strengthen Delivery Mechanisms
  </li>
  <li>
   Assure Sustainment Activities and Processes
  </li>
  <li>
   Manage Disposal and Final Disposition Activities throughout the System or Element Life Cycle
  </li>
 </ul>
 <h2 class="pt-3" id="detection">
  Detection
 </h2>
 <p>
  Use verification of distributed binaries through hash checking or other integrity checking mechanisms. Scan downloads for malicious signatures and attempt to test software and updates prior to deployment while taking note of potential suspicious activity. Perform physical inspection of hardware to look for potential tampering.
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
       <a class="external text" href="https://blog.avast.com/new-investigations-in-ccleaner-incident-point-to-a-possible-third-stage-that-had-keylogger-capacities" name="scite-1" rel="nofollow" target="_blank">
        Avast Threat Intelligence Team. (2018, March 8). New investigations into the CCleaner incident point to a possible third stage that had keylogger capacities. Retrieved March 15, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-2">
      <span class="scite-citation-text">
       <a class="external text" href="https://cloudblogs.microsoft.com/microsoftsecure/2018/03/07/behavior-monitoring-combined-with-machine-learning-spoils-a-massive-dofoil-coin-mining-campaign/" name="scite-2" rel="nofollow" target="_blank">
        Windows Defender Research. (2018, March 7). Behavior monitoring combined with machine learning spoils a massive Dofoil coin mining campaign. Retrieved March 20, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-3">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.commandfive.com/papers/C5_APT_SKHack.pdf" name="scite-3" rel="nofollow" target="_blank">
        Command Five Pty Ltd. (2011, September). SK Hack by an Advanced Persistent Threat. Retrieved April 6, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-4">
      <span class="scite-citation-text">
       <a class="external text" href="http://www.symantec.com/content/en/us/enterprise/media/security_response/whitepapers/the-elderwood-project.pdf" name="scite-4" rel="nofollow" target="_blank">
        O'Gorman, G., and McDonald, G.. (2012, September 6). The Elderwood Project. Retrieved February 15, 2018.
       </a>
      </span>
     </span>
    </li>
   </ol>
  </div>
  <div class="col">
   <ol start="5.0">
    <li>
     <span class="scite-citation" id="scite-5">
      <span class="scite-citation-text">
       <a class="external text" href="http://blog.talosintelligence.com/2017/09/avast-distributes-malware.html" name="scite-5" rel="nofollow" target="_blank">
        Brumaghin, E. et al. (2017, September 18). CCleanup: A Vast Number of Machines at Risk. Retrieved March 9, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-6">
      <span class="scite-citation-text">
       <a class="external text" href="http://www.intezer.com/evidence-aurora-operation-still-active-supply-chain-attack-through-ccleaner/" name="scite-6" rel="nofollow" target="_blank">
        Rosenberg, J. (2017, September 20). Evidence Aurora Operation Still Active: Supply Chain Attack Through CCleaner. Retrieved February 13, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-7">
      <span class="scite-citation-text">
       <a class="external text" href="https://www.mitre.org/sites/default/files/publications/se-guide-book-interactive.pdf" name="scite-7" rel="nofollow" target="_blank">
        The MITRE Corporation. (2014). MITRE Systems Engineering Guide. Retrieved April 6, 2018.
       </a>
      </span>
     </span>
    </li>
    <li>
     <span class="scite-citation" id="scite-8">
      <span class="scite-citation-text">
       <a class="external text" href="http://dx.doi.org/10.6028/NIST.IR.7622" name="scite-8" rel="nofollow" target="_blank">
        Boyens, J,. Et al.. (2002, October). Notional Supply Chain Risk Management Practices for Federal Information Systems. Retrieved April 6, 2018.
       </a>
      </span>
     </span>
    </li>
   </ol>
  </div>
 </div>
</div>
