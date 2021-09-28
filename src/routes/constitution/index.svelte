<script context="module">
	export const prerender = true;
</script>

<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">ALCOHOLICS ASSEMBLY CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: Basic Rules</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: Finances</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoOne)}>2.1 League Dues</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoTwo)}>2.2 Payout</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: League Ownership</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>3.1 Buy Out</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Rosters</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourOne)}>4.1 Positional Breakdown</h4>
	    <h4 class="noUnderscore clickable" on:click={() => goToSection(fourTwo)}>4.2 Future Notes</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: Scoring</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 Offense</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveTwo)}>5.2 Defense</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveThree)}>5.3 Kicking</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: Startup Auction Draft</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Section 7: Rookie Draft</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sevenOne)}>7.1 Draft Order</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(eight)}>Section 8: Free Agents</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(eightOne)}>8.1 FAAB</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(nine)}>Section 9: Trades</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(nineOne)}>9.1 Drug Rule</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(nineTwo)}>9.2 Trade Deadline</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(nineThree)}>9.3 Veto/Trade Process</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(ten)}>Section 10: Regular Season</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(eleven)}>Section 11: Playoffs</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(elevenOne)}>11.1 Playoff Seeding</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(elevenTwo)}>11.2 Playoff Tiebreakers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(elevenThree)}>11.2 Toilet Bowl</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(twelve)}>Section 12: Punishments</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(thirteen)}>Section 13: League Activity</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenOne)}>13.1 Tanking Policy</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenTwo)}>13.2 Communication Policy</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenThree)}>13.3 Social Media Policy</h4>
    
    <hr />

    <h2 class="sectionHeading" bind:this={one}>Section 1 Basic Rules</h2>
        <ul>
            <li>This is a DYNASTY league.  Owners are expected to commit to playing in this league for the foreseeable future.  The intent of this league is to give us a chance to continue to play fantasy football together for years to come in a more realistic football setting.  Turnover of ownership will result in the slow dismantlement of the league, so please consider this before committing.  If there is a problem with your continued ownership please notify the league and we will work on a way for you to stay or a replacement if necessary.</li>
            <li>AAFL is a 10 team league with no divisions.  This ensures the top players make the playoffs and draft order is easily seen.</li>
            <li>AAFL is a TE Premium league (1.0pts per reception) and will become a SuperFlex league starting with the 2022 season.</li>
            <li>The league season will begin from Week 1 of the NFL regular season and conclude with the championship ending at Week 17 (amended from Week 16 after the increase in games).</li>
            <li>Collusion will NOT be tolerated and will result in immediate proposals for expulsion to the league.</li>
            <li>If there are any rules that an owner would like to bring up for discussion, they may do so by:
                <ul>
                <li>Contacting the league commissioner with the rule they want changed</li>
                <li>Provide a solution to the rule change</li>
                <li>From here, a league vote will occur in which 51%+ must agree to the change for it to take effect immediately</li>
                <li>Vote will take place during Rookie/FA Draft Weekend</li>
                </ul>
            </li>
        </ul>
    <h2 class="sectionHeading" bind:this={two}>Section 2 Finances</h2>
    <h3 class="subSectionHeading" bind:this={twoOne}>2.1 League Dues</h3>
        <ul>
            <li>Owners are required to pay $125 to the league treasurer by the start of that year’s Rookie/FA Draft.</li>
            <li>Failure to pay or set up a payment plan with the league treasurer will result in forfeiting all winnings won that season, as well as a forfeiture of all draft picks until paid.</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={twoTwo}>2.2 Payout</h3>
        <ul>
            <li>1st Place: $705 + extra not used for league expenses</li>
            <li>2nd Place: $100</li>
            <li>3rd Place: $0</li>
            <li>Weekly Winner: $15/week</li>
            <li>Trophy Nameplate: $10</li>
        </ul>
    <h2 class="sectionHeading" bind:this={three}>Section 3 League Ownership</h2>
    <h3 class="subSectionHeading" bind:this={threeOne}>3.1 Buy Out</h3>
        <ul>
            <li>An owner that wants to leave the league must do so only after a new owner has been found AND the previous owner will pay the entry fee for the new owner for the following year.</li>
	    <li>If an owner no longer wants to participate in the AAFL, a new owner will be sought out by the entire league.</li>
            <li>If there are multiple options, a league vote will be held for all the nominations for possible new owners.  The owner with above a 50% acceptance rate will then be announced as the new owner barring acceptance.</li>
    	</ul>
    <h2 class="sectionHeading" bind:this={four}>Section 4 Rosters</h2>
    <h3 class="subSectionHeading" bind:this={fourOne}>4.1 Positional Breakdown</h3>
    <p class="bold">27 Total Players</p>
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>K</li>
        <li>D/ST</li>
    </ul>
    <p class="underscore">Bench</p>
    <ul>
        <li>17 active bench spots.</li>
    </ul>
    <p class="underscore">IR</p>
    <ul>
        <li>Each team will also have 2 Reserve spots for players that qualify.  These spots do not count as the 25 and if a player is activated off of the Reserve spot an active player must then be dropped to add them to your team.</li>
    </ul>
    <p class="underscore">Taxi Squad</p>
    <ul>
        <li>Taxi Squads will compile of 3 players of either ROOKIES or SOPHOMORES.</li>
        <li>Taxi Squads are locked during the season, only editable in the offseason or if an owner trades for a player on another owner’s Taxi Squad.</li>
        <li>If you activate a player on your own Taxi Squad, you can not move them back and must account for that space on your active roster.</li>
    </ul>
    <h3 class="subSectionHeading" bind:this={fourTwo}>4.2 Future Notes</h3>
    <p class="underscore">Super Flex</p>
    <ul>
        <li>Starting with the 2022 season, the FLEX position will be changed to a SuperFlex position.</li>
        <li>Owners will have the chance to start a QB, RB, WR, or TE in this spot.</li>
    </ul>
    <p class="underscore">Offseason</p>
    <ul>
        <li>In the Offseason, rosters will be expanded from 27 to 33 to accommodate new free agent pickups and drafted players.  There will be no IR spots available so all previous IR players will count towards the 30 roster limit.  Owners will cut rosters down from 33 to 27 by 11:59PM on the Sunday before Week One of the NFL season.</li>
    </ul>
    <p class="underscore">Retirement</p>
    <ul>
	<li>In the event that a player retires, the current owner may drop the player.  They reserve the right of first refusal for 1 year after they are dropped to pick them back up if the player in question re-joins the NFL.  If the player re-joins, that owner has 1 week to pick up that player.  After that week the player is officially a free agent and open to all owners.</li>
    </ul>
    <h2 class="sectionHeading" bind:this={five}>Section 5 Scoring</h2>
    <h3 class="subSectionHeading" bind:this={fiveOne}>5.1 Offense</h3>
        <ul>
            <li>Passing</li>
                <ul>
                    <li>Yards: 1pt = 25yds</li>
                    <li>Touchdowns: 4pts</li>
                    <li>Interceptions: -2pts</li>
                </ul>
            <li>Rushing</li>
                <ul>
                    <li>Yards: 1pt = 10yds</li>
                    <li>Touchdowns: 6pts</li>
                </ul>
            <li>Receiving</li>
                <ul>
                    <li>Receptions: 0.5pts</li>
                    <li>TE Receptions: 1.0pts</li>
                    <li>Yards: 1pt = 10yds</li>
                    <li>Touchdowns: 6pts</li>
                </ul>
            <li>Kick/Punt Returns</li>
                <ul>
                    <li>Touchdowns: 6pts</li>
                </ul>
            <li>Miscellaneous</li>
                <ul>
                    <li>Fumble Recovered for Touchdown: 6pts</li>
                    <li>2-Point Conversion: 2pts</li>
                    <li>Fumbles Lost: -2pts</li>
                </ul>
        </ul>
    <h3 class="subSectionHeading" bind:this={fiveTwo}>5.2 Defense</h3>
        <ul>
            <li>Sack: 1pt</li>
            <li>Interception: 2pts</li>
            <li>Fumble Recovered: 2pts</li>
            <li>Safety: 3pts</li>
            <li>Touchdown: 6pts</li>
            <li>2-Point Conversion Return: 2pts</li>
            <li>Blocked Kick: 1pt</li>
            <li>Return Touchdown: 6pts</li>
            <li>Points Allowed 0: 12pts</li>
            <li>Points Allowed 1-6: 10pts</li>
            <li>Points Allowed 7-13: 8pts</li>
            <li>Points Allowed 14-20: 6pts</li>
            <li>Points Allowed 21-27: 4pts</li>
            <li>Points Allowed 28-34: 2pts</li>
            <li>Points Allowed 35+: 0pts</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={fiveThree}>5.3 Kicking</h3>
        <ul>
            <li>PAT Made: 1pt</li>
            <li>PAT Missed: -1pt</li>
            <li>FG Made 0-19yds: 1pt</li>
            <li>FG Made 20-29yds: 2pts</li>
            <li>FG Made 30-39yds: 3pts</li>
            <li>FG Made 40-49yds: 4pts</li>
            <li>FG Made 50yds+: 5pts</li>
        </ul>

</div>

<!-- <div class="constitution">
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneOneOne)}>1.1.1 Position Maximums</h5>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneTwo)}>1.2 Trading</h4>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoOne)}>1.2.1 Trade Collusion</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoTwo)}>1.2.2 Lending Players Prohibition</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoFour)}>1.2.4 Trade Restrictions</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoFive)}>1.2.5 Veto/Trade Process</h5>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneThree)}>1.3 Waiver Wire</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: Drafting</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoOne)}>2.1 Draft Order</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoTwo)}>2.2 Rookie Drafts</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoThree)}>2.3 Draft Day Trades</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: Scoring System</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>3.1 Voting on Scoring System</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Postseason</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourOne)}>4.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourTwo)}>4.2 Playoff Tiebreakers</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: Tanking Policy</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 League Tanking Policy</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: Replacing Managers</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixOne)}>6.1 Removing Managers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixTwo)}>6.2 Replacing Managers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixThree)}>6.3 Replacement Incentive</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Section 7: League Finances</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sevenOne)}>7.1 League Dues</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixTwo)}>7.2 Payout</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixThree)}>7.3 Raising Dues</h4>
    
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 Roster Breakdown</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Breakdown</h3>
    
    <p>28 Total Players</p>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>FLEX (RB/WR)</li>
        <li>D/ST</li>
        <li>K</li>
    </ul>
    
    <p>18 Bench (Expanded by 5 between the keague draft and start of regular season)</p>

    <p>1 IR Spots (Player must be labeled as IR, Out, or Covid in the Sleeper App)</p>
    
        <h4 bind:this={oneOneOne}>1.1.1 Position Maximums</h4>
        
        <div class="subBlock">
            <table class="positionMaximums">
                <tr><td>QB</td><td class="right">3 active, 5 total</td></tr>
                <tr><td>RB</td><td class="right">20</td></tr>
                <tr><td>WR</td><td class="right">20</td></tr>
                <tr><td>TE</td><td class="right">10</td></tr>
                <tr><td>D/ST</td><td class="right">3</td></tr>
                <tr><td>K</td><td class="right">3</td></tr>
            </table>
        </div>


    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading</h3>
    
    <p>Trading of players and draft picks (up to 3 drafts away) are allowed. Trades will process immediately and will be reversed if vetoed or under investigation for collusion. Tradable assets include players, draft picks, and FAAB $.</p>
    
    <h4 bind:this={oneTwoOne}>1.2.1 Trade Collusion</h4>
    <div class="subBlock">
        <p>If any owners are suspected of accepting bribes/offering bribes to enhance their/another owners team via trade, trading any assets other than fantasy players, draft picks, FAAB $, or otherwise found guilty of engaging in any form of collusion*, all parties involved in the trade will be susceptible to punishment. The punishments will go as followed:</p>
        
        <ul>
            <li>First Offense – Immediate reduction of FAAB budget by 80%</li>
            <li>Second Offense – Immediate freeze on all transaction types for the next 18 weeks of regular season and playoff fantasy football games, including trades and waiver wire bids</li>
            <li>Third Offense – A league meeting of all members not involved in any of the improper trades/activity in question will take place to discuss next steps.</li>
        </ul>

        <p>All trades that are found guilty of collusion, will be reversed/denied. If the trade had affected the outcome of previous games, the results of those games will be revised.  </p>

        <p>*Collusion includes the organizing of veto votes against an acceptable trade.</p>

        <p>The commissioner will err on the side of letting owners manage their teams the way they see fit. Any collusion will need to be clear. The commissioner reserves the right to step in and at the very least assess the thinking of any team involved in a heavily lop-sided trade. </p>
    </div>

    <h4 bind:this={oneTwoTwo}>1.2.2 Lending Players Prohibition</h4>
    <div class="subBlock">
        <p>Any player traded from a team may not be re-acquired via trade within 6 weeks of the original trade. Any teams involved in this behavior will be subject to the aforementioned collusion punishments.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline will be set for the Saturday of the week 11 games of the NFL season.</p>
    </div>
    
    <h4 bind:this={oneTwoFour}>1.2.4 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You will not be able to trade draft picks that are more than 3 drafts away. For example, during the 2021 season you cannot trade any picks in or after the 2025 draft. You may only trade FAAB $ from the current season.</p>
    </div>
    
    <h4 bind:this={oneTwoFive}>1.2.5 Veto/Trade Process</h4>
    <div class="subBlock">
        <p>A total of 7 veto votes are required to veto a trade. Vetoes are only appropriate in instances of collusion or an egregious mismatch of value (i.e. CMC for a backup kicker). Not liking a trade does not warrant a veto.</p>
    </div>
    
    
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire</h3>
    
    <p>FAAB Waiver wire system. Each team will begin the season with $100. $0 bids are allowed. Bids will process Thursdays and Sundays at 9AM EST.</p>

    <p>FAAB budgets will reset each season in January.</p>
    
    
    <h2 class="sectionHeading" bind:this={two}>Section 2 Drafting</h2>
    
    <h3 bind:this={twoOne}>2.1 Draft Order</h3>
    <p>The draft order each year will be a linear draft in reverse order of the previous year’s regular season standings.</p>

    <h3 bind:this={twoTwo}>2.2 Rookie Drafts</h3>
    <p>Rokkie drafts will consist of 3 round of drafting, with 5 minutes alotted for each pick. To make room for the incoming players, benches will be expanded by (5) spots. These spots will be removed in mid-August, at which point you will need to have cut the necessary players.</p>
    <p>Any spots not filled during the draft, can be filled immediately afterwards from the waiver wire.</p>
    
    <h3 bind:this={twoThree}>2.3 Draft Day Trades</h3>
    <p>If a trade is being made during the draft, one or both parties can alert the commissioner to pause the draft to allow for extra time to negotiate the trade.</p>
    
    <h2 class="sectionHeading" bind:this={three}>Section 3 Scoring System</h2>

    <h3 bind:this={threeOne}>3.1 Scoring System</h3>
    <p>The league scoring system breakdown is listed on the Sleeper fantasy app (for the most part, it follows typical .5PPR Scoring). The scoring system will never change without a majority league vote.</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4 Postseason</h2>
    
    <h3 bind:this={fourOne}>4.1 Playoffs</h3>
    <p>At the end of the season 6 teams will make the playoffs. The first round of playoffs will commence in week 15. Each team that wins their division and the 4 wild card teams that finish with the best records, will receive a playoff berth. The 2 teams that win their division will receive a bye week in the first round of the playoffs. Each playoff matchup will only last one week and the winner will advance. Week 18 will not be used.</p>
    
    <h3 bind:this={fourTwo}>4.2 Seeding Tiebreakers</h3>
    <p>If two teams finish with the same record the tiebreakers will go as followed:</p>

    <ol>
        <li>Points For</li>
        <li>Head 2 Head Record</li>
        <li>Division Record</li>
        <li>Total Points Against</li>
        <li>Coin Flip</li>
        <li>Duel to the death</li>
    </ol>

    <h2 class="sectionHeading" bind:this={five}>Section 5 Tanking Policy</h2>
    
    <h3 bind:this={fiveOne}>5.1 League Tanking Policy</h3>
    <p>No team may intentionally leave starting roster spots empty. Any evidence of intentionally leaving roster spots empty in order to improve your draft position may be subject to punishment, including but not limited to the forfeiture of draft selections.</p>

    <h2 class="sectionHeading" bind:this={six}>Section 6 Replacing Managers</h2>
    
    <h3 bind:this={sixOne}>6.1 Removing Managers</h3>
    <p>Short of continuously failing to set a valid lineup, or confirmed collusion, no manager can be removed against their will. Participation, through the league chat, trade offers, and the waiver wire, is strongly encouraged but generally grounds for removal.</p>
    
    <h3 bind:this={sixTwo}>6.2 Replacing Managers</h3>
    <p>When a manager needs to be replaced, the commisiooners will try to find a suitable candidate with some connection to at least a portion of the existing managers. Priority will be placed on managers who are eager to take on a dynasty commitment and will be very active within the league.</p>
    
    <h3 bind:this={sixThree}>6.3 Replacement Incentive</h3>
    <p>In the event that a manager chooses to quit the league or is removed by a comissioner, an incoming manager is offered a 50% reductioon on their first year buy-in.</p>

    <h2 class="sectionHeading" bind:this={seven}>Section 7 League Finances</h2>
    
    <h3 bind:this={sevenOne}>7.1 League Dues</h3>
    <p>League dues are set at {dues}$. Dues are collected through <a href="https://www.leaguesafe.com/league/3949641">LeagueSafe</a> and collection will be sent out no later than the first of August. All managers must be fully paid up before the start of regular season. In the event that a manager fails to pay before the deadline, a 10% penalty will be addd to their payment and will go towards the payouts at the end of the year.</p>
    
    <h3 bind:this={sevenTwo}>7.2 Payout</h3>
    <p>League payout is structured as follows:</p>
    <ul>
        <li>1st place: {dues * 8}$</li>
        <li>2nd place: {dues * 3}$</li>
        <li>3rd place: {dues}$</li>
    </ul>
    <p>In the event that a manager was fined due to late payment, their extra fee will be added to the winner's payout. Similarly, if new managers come into the league and the payout is smaller, the difference will come out of the winner's prize.</p>
    
    <h3 bind:this={sevenThree}>7.3 Raising Dues</h3>
    <p>A ⅔ majority vote is required in order to raise league dues. In the event that a manager is no longer financially comfortable with the buyin, finding a co-manager to split the cost is reccomended.</p>

</div> -->
