<script context="module">
	export const prerender = true;
</script>

<script>
    import { dues } from '$lib/utils/helper';
    let one;
    let two, twoOne;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne, fiveTwo, fiveThree;
    let six;
    let seven, sevenOne;
    let eight, eightOne;
    let nine, nineOne, nineTwo, nineThree;
    let ten;
    let eleven, elevenOne, elevenTwo, elevenThree;
    let twelve;
    let thirteen, thirteenOne, thirteenTwo, thirteenThree, thirteenFour
    let fourteen;

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
        	<h4 class="noUnderscore clickable" on:click={() => goToSection(elevenThree)}>11.3 Toilet Bowl</h4>
    	<h3 class="noUnderscore clickable" on:click={() => goToSection(twelve)}>Section 12: Punishments</h3>
    	<h3 class="noUnderscore clickable" on:click={() => goToSection(thirteen)}>Section 13: League Activity</h3>
        	<h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenOne)}>13.1 Tanking Policy</h4>
        	<h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenTwo)}>13.2 Punishment Policy</h4>
        	<h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenThree)}>13.3 Social Media Policy</h4>
        	<h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenFour)}>13.4 League Activity Policy</h4>
    	<h3 class="noUnderscore clickable" on:click={() => goToSection(fourteen)}>Section 14: League Accessories</h3>

	<hr />

	<h2 class="sectionHeading" bind:this={one}>Section 1: Basic Rules</h2>
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
    	<h2 class="sectionHeading" bind:this={two}>Section 2: Finances</h2>
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
	<h2 class="sectionHeading" bind:this={three}>Section 3: League Ownership</h2>
    	<h3 class="subSectionHeading" bind:this={threeOne}>3.1 Buy Out</h3>
        <ul>
            <li>An owner that wants to leave the league must do so only after a new owner has been found AND the previous owner will pay the entry fee for the new owner for the following year.</li>
	    <li>If an owner no longer wants to participate in the AAFL, a new owner will be sought out by the entire league.</li>
            <li>If there are multiple options, a league vote will be held for all the nominations for possible new owners.  The owner with above a 50% acceptance rate will then be announced as the new owner barring acceptance.</li>
    	</ul>
    	<h2 class="sectionHeading" bind:this={four}>Section 4: Rosters</h2>
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
	<h2 class="sectionHeading" bind:this={five}>Section 5: Scoring</h2>
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
    	<h2 class="sectionHeading" bind:this={six}>Section 6: Startup Auction Draft</h2>
        <ul>
            <li>A startup auction draft will be held on September 3, 2017 to begin our new transition from Re-Draft FFL to a Dynasty FFL.  Location is at Manny Savas’ house.  Time of start will be determined day-of.  This will be a live draft.</li>
            <li>Each owner will be given a salary of $200 to fill out the team as they please.</li>
            <li>Players will be nominated in order of their finish in the 2017 March Madness Bracket.</li>
            <li>Bidding Process:
                <ul>
                    <li>A player is nominated with a bid of at least $0, in which other owners are then allowed to bid themselves</li>
                    <li>There is no minimum bid, so you are allowed to bid $0</li>
                    <li>A countdown clock of 1:30 will thus begin</li>
                    <li>Once the clock is under :10, the clock will reset to :10 with every following bid</li>
                    <li>Owners will be allowed to bid until there are no other bidders left, in which they are awarded that player</li>
                    <li>If all owners reach $0 without all rosters filled, it will begin a standard draft with all owners still in need of players until all rosters are completely filled out</li>
                </ul>
            </li>
            <li>Once completed, the league commissioner will input the results into the league platform.</li>
        </ul>
	
	
	
	<h2 class="sectionHeading" bind:this={seven}>Section 7: Rookie Draft</h2>
        <ul>
            <li>he R/FA draft will take place the following Sunday directly after the NFL draft or otherwise discussed.  LEAGUE WINNER PLANS THIS WEEKEND.</li>
            <li>This will be a 5 round draft.</li>
            <li>All new NFL rookies will be available in this draft, along with all Free Agents from the previous fantasy season.</li>
            <li>One week before draft day, owners must have open spots for all future draft picks they have.  If an owner has more picks than can legally roster, they must either cut players or forfeit picks in order to not go over their 33 man roster limit.  All players cut will be immediately available in the R/FA draft and picks forfeited will be skipped during the draft.</li>
            <li>The draft will NOT be a snake draft. It will be a standard draft (i.e. NFL draft).</li>
            <li>If a team has traded a pick, that pick will then be given to the correct team once their draft order is in place.</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={sevenOne}>7.1 Draft Order</h3>
        <ul>
            <li>1st= 10th place in regular season</li>
            <li>2nd= 9th place in regular season</li>
            <li>3rd= 8th place in regular season</li>
            <li>4th= 7th place in regular season</li>
            <li>5th= Winner of the 5th place game</li>
            <li>6th= Loser of the 5th place game</li>
            <li>7th= Loser of the 3rd place game</li>
            <li>8th= Winner of the 3rd place game</li>
            <li>9th= Loser of the championship game</li>
            <li>10th= Winner of the championship game</li>
        </ul>
    	<h2 class="sectionHeading" bind:this={eight}>Section 8 Free Agents</h2>
        <ul>
            <li>All players not drafted will become free agents after the draft.</li>
            <li>Waivers are ran early Wednesday morning (via Sleeper standard).</li>
            <li>FAAB during offseason pickups will be taken from your yearly FAAB budget.</li>
            <li>Free agents will exist throughout the year.  They will be locked for the week at the start of their game.</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={eightOne}>8.1 FAAB</h3>
        <ul>
            <li>We will be using a FAAB for any free agent pickups</li>
            <li>Each team will have $100 FAAB points/year to spend on free agent pickups</li>
            <li>This is a blind bid where the highest bid is awarded to the player, and all other bids are then given back to their respective teams</li>
            <li>Bids are accepted starting early Tuesday morning until Wednesday at 6am</li>
        </ul>
    	<h2 class="sectionHeading" bind:this={nine}>Section 9 Trades</h2>
        <ul>
            <li>Trades of players & draft picks both will be allowed.</li>
            <li>Trades may only involve players & picks.</li>
            <li>Draft picks involved in a trade will only be allowed up to 2 years out.  This prevents owners from trading draft picks so far in the future that can affect other/new owners if they quit the league.</li>
            <li>Trade of future draft picks of equal rounds is considered a bet, resulting in a nullification of that trade (i.e. trading next years first round picks straight up before the picks are determined).</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={nineOne}>9.1 Drug Rule</h3>
        <ul>
            <li>If a trade is made with one or more owners under the influence of a drug (alcohol, weed, medicine, etc) or in an impaired state, that trade will stay on the table for 24 hours</li>
            <li>This allows for all trades to be made in a sober state by all parties to keep fairness</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={nineTwo}>9.2 Trade Deadline</h3>
        <ul>
            <li>Trade Deadline: Week 13 (amended to the last week of the regular season)</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={nineThree}>9.3 Veto/Trade Process</h3>
        <ul>
            <li>All trades will be accepted by the league UNLESS an owner views this as unfair to the league or collusion is taking place</li>
            <li>An owner can request a league vote, with the commissioner heading the vote</li>
            <li>If the trade is accepted (50%+) , it will process immediately upon acceptance.  If the trade is vetoed, the trade will immediately be denied and owners will have to work out a new trade</li>
            <li>Vetos will only be accepted if there is outstanding evidence that the trade is greatly unbalanced or collusion is at play</li>
        </ul>
    	<h2 class="sectionHeading" bind:this={ten}>Section 10 Regular Season</h2>
        <ul>
            <li>The regular season will last from Week 1 until Week 13 of the NFL season.</li>
            <li>Each team’s schedule will be randomly created by the platform we play on at season’s start.</li>
            <li>There are no ties in the AAFL.  If a tie is to occur, the total amount of bench points will be the tiebreaker of the matchup.</li>
        </ul>
    	<h2 class="sectionHeading" bind:this={eleven}>Section 11 Playoffs</h2>
        <ul>
            <li>The playoffs will last from Week 14 until Week 17 of the NFL season.</li>
            <li>All playoff matchups are 1 week long.</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={elevenOne}>11.1 Playoff Seeding</h3>
        <ul>
            <li>The top 6 teams will make the playoffs</li>
            <li>First Round:
                <ul>
                    <li>The #1 and #2 teams will receive a bye</li>
                    <li>#3 vs #6</li>
                    <li>#4 vs #5</li>
                </ul>
            </li>
            <li>Second Round:
                <ul>
                    <li>#1 vs #4/5 </li>
                    <li>#2 vs #3/6</li>
                </ul>
            </li>
            <li>Championship:
                <ul>
                    <li>#1/4/5 vs #2/3/6</li>
                </ul>
            </li>
            <li>3rd Place Matchup:
                <ul>
                    <li>Both losers of the 2nd round will face each other in a 3rd place matchup the same 2 weeks as the championship.  The Winner of this matchup will be awarded the 7th pick in the following year’s draft</li>
                    <li>Ran as a Best Ball matchup (see Toilet Bowl for more details)</li>
                </ul>
            </li>
            <li>5th Place Matchup:
                <ul>
                    <li>Both losers in the 1st round will face each other in a 5th place matchup the same 2 weeks as the championship.  The Winner of this matchup will be awarded the 5th pick in the following year’s draft</li>
                    <li>Ran as a Best Ball matchup (see Toilet Bowl for more details)</li>
                </ul>
            </li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={elevenTwo}>11.2 Playoff Tiebreakers</h3>
        <ul>
            <li>Commish will need to manually edit this until Sleeper updates this</li>
            <li>For teams with similar records, the tie breaker order goes as follows:
                <ol>
                    <li>H2H Record (or combined record against all tied teams if 3+ tied)</li>
                    <li>Points For</li>
                </ol>
            </li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={elevenThree}>11.3 Toilet Bowl</h3>
        <ul>
            <li>Will now be ran as a Best Ball competition in which the commissioner will revert back on Tuesday and decide which players will count for each team</li>
            <li>This will help prevent tanking, and allow the true worst teams the best draft picks in efforts to keep a solid competitive balance</li>
        </ul>
    	<h2 class="sectionHeading" bind:this={twelve}>Section 12: Punishments</h2>
        <ul>
            <li>The owner that finishes in 10th place of the regular season will be required to perform the punishment</li>
            <li>Each year, the commissioner will send out a Google Form for all 10 owners to submit their punishment idea(s) for the upcoming season:
                <ul>
                    <li>Each owner is required to submit 1, but may submit a second punishment idea as well in case their first idea has already been submitted</li>
                    <li>The commissioner will reveal the 10 punishment ideas during Week 1</li>
                    <li>The 10th place finisher must choose 1 of the ideas submitted to complete, but are not allowed to pick their own</li>
                </ul>
            </li>
            <li>Failure to accomplish punishment by kickoff of the first NFL regular season game of the following year will result in the following until the punishment is successfully completed:
                <ul>
                    <li>All trading will be disabled</li>
                    <li>All adds/drops will be disabled</li>
                    <li>You will not be eligible to make playoffs</li>
                    <li>All future picks will be forfeited</li>
                </ul>
            </li>
        </ul>
    	<h2 class="sectionHeading" bind:this={thirteen}>Section 13: League Activity</h2>
    	<h3 class="subSectionHeading" bind:this={thirteenOne}>13.1 Tanking Policy</h3>
        <ul>
            <li>Tanking will not be tolerated</li>
            <li>If an owner believes another is tanking, they may bring it up for discussion with the commissioner</li>
            <li>If the commissioner believes they are purposely tanking, they will approach the league with further steps</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={thirteenTwo}>13.2 Punishment Policy</h3>
        <ul>
            <li>The failure to acknowledge and communicate within the league will not be tolerated</li>
            <li>1st Offense: Warning</li>
            <li>2nd Offense: Warning and loss of future mid-level draft pick</li>
            <li>3rd Offense: Removal of owner pending league vote</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={thirteenThree}>13.3 Social Media Policy</h3>
        <ul>
            <li>Facebook is ONLY used for polls, important news/notes, and all other matters regarding the control of the league</li>
            <li>GroupMe is ONLY used for trash talk and everyday talk</li>
            <li>Twitter will be accessible by all owners at their request.  Username is @OfficialAAFL and the password is dave4commish2020.  There will NOT be any profanity or inappropriate use.  If someone has a complaint about a post, they may bring it up for a discussion to be taken down.  Action will then be taken if needed</li>
            <li>Website will be used to portray the league to the public.  NSFW images and words are not allowed to be posted and all owner’s wishes will be respected</li>
            <li>Commissioner and other admins allowed will monitor both outlets to make sure everything runs smoothly</li>
        </ul>
    	<h3 class="subSectionHeading" bind:this={thirteenFour}>13.4 League Activity Policy</h3>
        <ul>
            <li>League activity is required by all owners.  All owners are expected to following the following guidelines</li>
            <li>Set weekly lineups to the best of their ability (NO tanking, teams must start players to the best of their ability)</li>
            <li>Acknowledge trades when approached and accept/decline/discuss them</li>
            <li>Participate in all league votes and polls</li>
            <li>Draft their own players</li>
        </ul>
    	<h2 class="sectionHeading" bind:this={fourteen}>Section 14: League Accessories</h2>
        <ul>
            <li>2021 Rate My League PDF Breakdown: https://ratemyleague.com/rml/pdfs/320BD1A57E3FB84EB9C21FE9D0ADD940.pdf</li>
            <li>2020 Dynasty Dude Preview Podcast: https://drive.google.com/file/d/19bx8zyyThrprNAt9TDTnOgzxYHInUw3q/view?usp=sharing</li>
            <li>2020 AAFL Magazine: https://anyflip.com/yiusn/pxjv/?fbclid=IwAR014ETb8zW7zyiGK8k-TmvFpBvfJ50pNK0xKy5-Jyqqs6wxXtw7B22fbRo</li>
            <li>2018 Newsletter: https://docs.google.com/document/d/12xg6VArFU2UEON7S--nT5BkAja8FA8BwP0C0L_vtoxI/edit?fbclid=IwAR0rUrH0a4ZTMCQ7IP44XZwrObG1ZxCb-DKYQR0ZHT89fGo5q7hHyY3rwak</li>
            <li>2017 Magazine: https://anyflip.com/elbr/nqfs?fbclid=IwAR02tluCv1brITDRqSDrgzskt67E9jDXFWKd2S7BE56GHD-Oar3tKGQQ0YM</li>
            <li>Facebook: https://www.facebook.com/groups/340428833055185</li>
            <li>Twitter: https://twitter.com/OfficialAAFL</li>
        </ul>
</div>


<!-- <div class="constitution">
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
        <h4 class="noUnderscore clickable" on:click={() => goToSection(elevenThree)}>11.3 Toilet Bowl</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(twelve)}>Section 12: Punishments</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(thirteen)}>Section 13: League Activity</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenOne)}>13.1 Tanking Policy</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenTwo)}>13.2 Punishment Policy</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenThree)}>13.3 Social Media Policy</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(thirteenFour)}>13.4 League Activity Policy</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(fourteen)}>Section 14: League Accessories</h3>

    <hr />

    <h2 class="sectionHeading" bind:this={one}>Section 1: Basic Rules</h2>
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
    <h2 class="sectionHeading" bind:this={two}>Section 2: Finances</h2>
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
    <h2 class="sectionHeading" bind:this={three}>Section 3: League Ownership</h2>
    <h3 class="subSectionHeading" bind:this={threeOne}>3.1 Buy Out</h3>
        <ul>
            <li>An owner that wants to leave the league must do so only after a new owner has been found AND the previous owner will pay the entry fee for the new owner for the following year.</li>
	    <li>If an owner no longer wants to participate in the AAFL, a new owner will be sought out by the entire league.</li>
            <li>If there are multiple options, a league vote will be held for all the nominations for possible new owners.  The owner with above a 50% acceptance rate will then be announced as the new owner barring acceptance.</li>
    	</ul>
    <h2 class="sectionHeading" bind:this={four}>Section 4: Rosters</h2>
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
    <h2 class="sectionHeading" bind:this={five}>Section 5: Scoring</h2>
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
    <h2 class="sectionHeading" bind:this={six}>Section 6: Startup Auction Draft</h2>
        <ul>
            <li>A startup auction draft will be held on September 3, 2017 to begin our new transition from Re-Draft FFL to a Dynasty FFL.  Location is at Manny Savas’ house.  Time of start will be determined day-of.  This will be a live draft.</li>
            <li>Each owner will be given a salary of $200 to fill out the team as they please.</li>
            <li>Players will be nominated in order of their finish in the 2017 March Madness Bracket.</li>
            <li>Bidding Process:
                <ul>
                    <li>A player is nominated with a bid of at least $0, in which other owners are then allowed to bid themselves</li>
                    <li>There is no minimum bid, so you are allowed to bid $0</li>
                    <li>A countdown clock of 1:30 will thus begin</li>
                    <li>Once the clock is under :10, the clock will reset to :10 with every following bid</li>
                    <li>Owners will be allowed to bid until there are no other bidders left, in which they are awarded that player</li>
                    <li>If all owners reach $0 without all rosters filled, it will begin a standard draft with all owners still in need of players until all rosters are completely filled out</li>
                </ul>
            </li>
            <li>Once completed, the league commissioner will input the results into the league platform.</li>
        </ul>
    <h2 class="sectionHeading" bind:this={seven}>Section 7: Rookie Draft</h2>
        <ul>
            <li>he R/FA draft will take place the following Sunday directly after the NFL draft or otherwise discussed.  LEAGUE WINNER PLANS THIS WEEKEND.</li>
            <li>This will be a 5 round draft.</li>
            <li>All new NFL rookies will be available in this draft, along with all Free Agents from the previous fantasy season.</li>
            <li>One week before draft day, owners must have open spots for all future draft picks they have.  If an owner has more picks than can legally roster, they must either cut players or forfeit picks in order to not go over their 33 man roster limit.  All players cut will be immediately available in the R/FA draft and picks forfeited will be skipped during the draft.</li>
            <li>The draft will NOT be a snake draft. It will be a standard draft (i.e. NFL draft).</li>
            <li>If a team has traded a pick, that pick will then be given to the correct team once their draft order is in place.</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={sevenOne}>7.1 Draft Order</h3>
        <ul>
            <li>1st= 10th place in regular season</li>
            <li>2nd= 9th place in regular season</li>
            <li>3rd= 8th place in regular season</li>
            <li>4th= 7th place in regular season</li>
            <li>5th= Winner of the 5th place game</li>
            <li>6th= Loser of the 5th place game</li>
            <li>7th= Loser of the 3rd place game</li>
            <li>8th= Winner of the 3rd place game</li>
            <li>9th= Loser of the championship game</li>
            <li>10th= Winner of the championship game</li>
        </ul>
    <h2 class="sectionHeading" bind:this={eight}>Section 8 Free Agents</h2>
        <ul>
            <li>All players not drafted will become free agents after the draft.</li>
            <li>Waivers are ran early Wednesday morning (via Sleeper standard).</li>
            <li>FAAB during offseason pickups will be taken from your yearly FAAB budget.</li>
            <li>Free agents will exist throughout the year.  They will be locked for the week at the start of their game.</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={eightOne}>8.1 FAAB</h3>
        <ul>
            <li>We will be using a FAAB for any free agent pickups</li>
            <li>Each team will have $100 FAAB points/year to spend on free agent pickups</li>
            <li>This is a blind bid where the highest bid is awarded to the player, and all other bids are then given back to their respective teams</li>
            <li>Bids are accepted starting early Tuesday morning until Wednesday at 6am</li>
        </ul>
    <h2 class="sectionHeading" bind:this={nine}>Section 9 Trades</h2>
        <ul>
            <li>Trades of players & draft picks both will be allowed.</li>
            <li>Trades may only involve players & picks.</li>
            <li>Draft picks involved in a trade will only be allowed up to 2 years out.  This prevents owners from trading draft picks so far in the future that can affect other/new owners if they quit the league.</li>
            <li>Trade of future draft picks of equal rounds is considered a bet, resulting in a nullification of that trade (i.e. trading next years first round picks straight up before the picks are determined).</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={nineOne}>9.1 Drug Rule</h3>
        <ul>
            <li>If a trade is made with one or more owners under the influence of a drug (alcohol, weed, medicine, etc) or in an impaired state, that trade will stay on the table for 24 hours</li>
            <li>This allows for all trades to be made in a sober state by all parties to keep fairness</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={nineTwo}>9.2 Trade Deadline</h3>
        <ul>
            <li>Trade Deadline: Week 13 (amended to the last week of the regular season)</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={nineThree}>9.3 Veto/Trade Process</h3>
        <ul>
            <li>All trades will be accepted by the league UNLESS an owner views this as unfair to the league or collusion is taking place</li>
            <li>An owner can request a league vote, with the commissioner heading the vote</li>
            <li>If the trade is accepted (50%+) , it will process immediately upon acceptance.  If the trade is vetoed, the trade will immediately be denied and owners will have to work out a new trade</li>
            <li>Vetos will only be accepted if there is outstanding evidence that the trade is greatly unbalanced or collusion is at play</li>
        </ul>
    <h2 class="sectionHeading" bind:this={ten}>Section 10 Regular Season</h2>
        <ul>
            <li>The regular season will last from Week 1 until Week 13 of the NFL season.</li>
            <li>Each team’s schedule will be randomly created by the platform we play on at season’s start.</li>
            <li>There are no ties in the AAFL.  If a tie is to occur, the total amount of bench points will be the tiebreaker of the matchup.</li>
        </ul>
    <h2 class="sectionHeading" bind:this={eleven}>Section 11 Playoffs</h2>
        <ul>
            <li>The playoffs will last from Week 14 until Week 17 of the NFL season.</li>
            <li>All playoff matchups are 1 week long.</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={elevenOne}>11.1 Playoff Seeding</h3>
        <ul>
            <li>The top 6 teams will make the playoffs</li>
            <li>First Round:
                <ul>
                    <li>The #1 and #2 teams will receive a bye</li>
                    <li>#3 vs #6</li>
                    <li>#4 vs #5</li>
                </ul>
            </li>
            <li>Second Round:
                <ul>
                    <li>#1 vs #4/5 </li>
                    <li>#2 vs #3/6</li>
                </ul>
            </li>
            <li>Championship:
                <ul>
                    <li>#1/4/5 vs #2/3/6</li>
                </ul>
            </li>
            <li>3rd Place Matchup:
                <ul>
                    <li>Both losers of the 2nd round will face each other in a 3rd place matchup the same 2 weeks as the championship.  The Winner of this matchup will be awarded the 7th pick in the following year’s draft</li>
                    <li>Ran as a Best Ball matchup (see Toilet Bowl for more details)</li>
                </ul>
            </li>
            <li>5th Place Matchup:
                <ul>
                    <li>Both losers in the 1st round will face each other in a 5th place matchup the same 2 weeks as the championship.  The Winner of this matchup will be awarded the 5th pick in the following year’s draft</li>
                    <li>Ran as a Best Ball matchup (see Toilet Bowl for more details)</li>
                </ul>
            </li>
        </ul>
    <h3 class="subSectionHeading" bind:this={elevenTwo}>11.2 Playoff Tiebreakers</h3>
        <ul>
            <li>Commish will need to manually edit this until Sleeper updates this</li>
            <li>For teams with similar records, the tie breaker order goes as follows:
                <ol>
                    <li>H2H Record (or combined record against all tied teams if 3+ tied)</li>
                    <li>Points For</li>
                </ol>
            </li>
        </ul>
    <h3 class="subSectionHeading" bind:this={elevenThree}>11.3 Toilet Bowl</h3>
        <ul>
            <li>Will now be ran as a Best Ball competition in which the commissioner will revert back on Tuesday and decide which players will count for each team</li>
            <li>This will help prevent tanking, and allow the true worst teams the best draft picks in efforts to keep a solid competitive balance</li>
        </ul>
    <h2 class="sectionHeading" bind:this={twelve}>Section 12: Punishments</h2>
        <ul>
            <li>The owner that finishes in 10th place of the regular season will be required to perform the punishment</li>
            <li>Each year, the commissioner will send out a Google Form for all 10 owners to submit their punishment idea(s) for the upcoming season:
                <ul>
                    <li>Each owner is required to submit 1, but may submit a second punishment idea as well in case their first idea has already been submitted</li>
                    <li>The commissioner will reveal the 10 punishment ideas during Week 1</li>
                    <li>The 10th place finisher must choose 1 of the ideas submitted to complete, but are not allowed to pick their own</li>
                </ul>
            </li>
            <li>Failure to accomplish punishment by kickoff of the first NFL regular season game of the following year will result in the following until the punishment is successfully completed:
                <ul>
                    <li>All trading will be disabled</li>
                    <li>All adds/drops will be disabled</li>
                    <li>You will not be eligible to make playoffs</li>
                    <li>All future picks will be forfeited</li>
                </ul>
            </li>
        </ul>
    <h2 class="sectionHeading" bind:this={thirteen}>Section 13: League Activity</h2>
    <h3 class="subSectionHeading" bind:this={thirteenOne}>13.1 Tanking Policy</h3>
        <ul>
            <li>Tanking will not be tolerated</li>
            <li>If an owner believes another is tanking, they may bring it up for discussion with the commissioner</li>
            <li>If the commissioner believes they are purposely tanking, they will approach the league with further steps</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={thirteenTwo}>13.2 Punishment Policy</h3>
        <ul>
            <li>The failure to acknowledge and communicate within the league will not be tolerated</li>
            <li>1st Offense: Warning</li>
            <li>2nd Offense: Warning and loss of future mid-level draft pick</li>
            <li>3rd Offense: Removal of owner pending league vote</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={thirteenThree}>13.3 Social Media Policy</h3>
        <ul>
            <li>Facebook is ONLY used for polls, important news/notes, and all other matters regarding the control of the league</li>
            <li>GroupMe is ONLY used for trash talk and everyday talk</li>
            <li>Twitter will be accessible by all owners at their request.  Username is @OfficialAAFL and the password is dave4commish2020.  There will NOT be any profanity or inappropriate use.  If someone has a complaint about a post, they may bring it up for a discussion to be taken down.  Action will then be taken if needed</li>
            <li>Website will be used to portray the league to the public.  NSFW images and words are not allowed to be posted and all owner’s wishes will be respected</li>
            <li>Commissioner and other admins allowed will monitor both outlets to make sure everything runs smoothly</li>
        </ul>
    <h3 class="subSectionHeading" bind:this={thirteenFour}>13.4 League Activity Policy</h3>
        <ul>
            <li>League activity is required by all owners.  All owners are expected to following the following guidelines</li>
            <li>Set weekly lineups to the best of their ability (NO tanking, teams must start players to the best of their ability)</li>
            <li>Acknowledge trades when approached and accept/decline/discuss them</li>
            <li>Participate in all league votes and polls</li>
            <li>Draft their own players</li>
        </ul>
    <h2 class="sectionHeading" bind:this={fourteen}>Section 14: League Accessories</h2>
        <ul>
            <li>2021 Rate My League PDF Breakdown: https://ratemyleague.com/rml/pdfs/320BD1A57E3FB84EB9C21FE9D0ADD940.pdf</li>
            <li>2020 Dynasty Dude Preview Podcast: https://drive.google.com/file/d/19bx8zyyThrprNAt9TDTnOgzxYHInUw3q/view?usp=sharing</li>
            <li>2020 AAFL Magazine: https://anyflip.com/yiusn/pxjv/?fbclid=IwAR014ETb8zW7zyiGK8k-TmvFpBvfJ50pNK0xKy5-Jyqqs6wxXtw7B22fbRo</li>
            <li>2018 Newsletter: https://docs.google.com/document/d/12xg6VArFU2UEON7S--nT5BkAja8FA8BwP0C0L_vtoxI/edit?fbclid=IwAR0rUrH0a4ZTMCQ7IP44XZwrObG1ZxCb-DKYQR0ZHT89fGo5q7hHyY3rwak</li>
            <li>2017 Magazine: https://anyflip.com/elbr/nqfs?fbclid=IwAR02tluCv1brITDRqSDrgzskt67E9jDXFWKd2S7BE56GHD-Oar3tKGQQ0YM</li>
            <li>Facebook: https://www.facebook.com/groups/340428833055185</li>
            <li>Twitter: https://twitter.com/OfficialAAFL</li>
        </ul>
</div> -->
