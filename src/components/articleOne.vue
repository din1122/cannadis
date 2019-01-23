<template>
	<div>

		<v-layout row wrap>
			<v-flex xs12 xl4 @click="dialog = true">
				<div class="img-box">
					<img :src="require('@/assets/medicne.png')" alt="home-1-cannabis" class="article-img">
				</div>
			</v-flex>
			<v-flex xs10 xl8 class="article-text" pl-3>
				<span @click="dialog = true" class="display-1  article-title">Cannabis as a medicne</span><br><br>
				<p @click="dialog = true">
					Medical cannabis,is cannabis and cannabinoids that are recommended by doctors for their patients. Evidence
					suggests that cannabis can reduce nausea and vomiting during chemotherapy, improve appetite in people with
					HIV/AIDS, and reduce chronic pain and muscle spasms.The Cannabis plant has a history of medicinal use dating back
					thousands of years in many cultures .Medical cannabis can be administered through a variety of methods, including
					capsules, lozenges, tinctures, dermal patches, oral or dermal sprays, cannabis edibles, and vaporizing or smoking
					dried buds.
				</p><br>
				<p><span>Publish By:</span> <span class="aurtor"> Din ashkneazi</span> | <span> Date:</span> <span>24 Oct</span>
				</p>
			</v-flex>
		</v-layout>



		<v-dialog v-model="dialog">
			<v-container fluid pa-0>

				<v-card>
					<v-icon class="fixed pa-3 right" @click="dialog= false">close</v-icon>
					<v-flex pa-3>
						<v-card-title>
						<img :src="require('@/assets/medicne.png')" alt="home-1-cannabis" class="article-img-box pb-4">
						<span class="display-3 article-main-title">
						Cannabis as a medicne</span></v-card-title>
						<v-card-text>
							<p>
								The term <em>medical marijuana</em> refers to using the whole, unprocessed marijuana plant or its basic
								extracts to treat symptoms of illness and other conditions. The U.S. Food and Drug Administration (FDA) has not
								recognized or approved the marijuana plant as medicine.
							</p>

							<p>
								However, scientific study of the chemicals in marijuana, called <em>cannabinoids</em>, has led to two
								FDA-approved medications that contain cannabinoid chemicals in pill form. Continued research may lead to more
								medications.
							</p>

							<p>
								Because the marijuana plant contains chemicals that may help treat a range of illnesses and symptoms, many
								people argue that it should be legal for medical purposes. In fact, a growing number of states have legalized
								marijuana for medical use.
							</p>

							<h2>
								Why isn&rsquo;t the marijuana plant an FDA-approved medicine?
							</h2>

							<p>
								The FDA requires carefully conducted studies (clinical trials) in hundreds to thousands of human subjects to
								determine the benefits and risks of a possible medication. So far, researchers haven&#39;t conducted enough
								large-scale clinical trials that show that the benefits of the marijuana plant (as opposed to its cannabinoid
								ingredients) outweigh its risks in patients it&#39;s meant to treat.
							</p>

							<p>
								Read more about the various physical, mental, and behavioral effects of marijuana in our <em><a href="https://www.drugabuse.gov/publications/drugfacts/marijuana">Marijuana
										DrugFacts</a></em>.
							</p>

							<div>
								<h3>
									Can Medical Marijuana Legalization Decrease Prescription Opioid Problems?
								</h3>

								<p>
									Some studies have suggested that medical marijuana legalization might be associated with decreased
									prescription opioid use and overdose deaths, but researchers don&#39;t have enough evidence yet to confirm
									this finding. For example, one study found that Medicare Part D prescriptions filled for all opioids decreased
									in states with medical marijuana laws.<a href="#references"><sup>1</sup></a> Another study examined Medicaid
									prescription data and found that medical marijuana laws and adult-use marijuana laws were associated with
									lower opioid prescribing rates (5.88 percent and 6.88 percent lower, respectively).<a href="#references"><sup>2</sup></a>

									<p>
										Additionally, one NIDA-funded study suggested a link between medical marijuana legalization and fewer
										overdose deaths from prescription opioids.<a href="#references"><sup>3</sup></a> These studies, however, are
										population-based and can&rsquo;t show that medical marijuana legalization caused the decrease in deaths or
										that pain patients changed their drug-taking behavior.<a href="#references"><sup>4,5</sup></a> A more
										detailed NIDA-funded analysis showed that legally protected medical marijuana dispensaries, not just medical
										marijuana laws, were also associated with a decrease in the following:<a href="#references"><sup>6</sup></a>

										<ul>
											<li>
												opioid prescribing
											</li>
											<li>
												self-reports of opioid misuse
											</li>
											<li>
												treatment admissions for opioid addiction
											</li>
										</ul>

										<p>
											Additionally, some data suggests that medical marijuana treatment may reduce the opioid dose prescribed for
											pain patients,<a href="#references"><sup>7,8</sup></a> while another recent NIH-funded study suggests that
											cannabis use appears to increase the risk of developing and opioid use disorder.<a href="#references"><sup>9</sup></a>
											NIDA is funding additional studies to determine the link between medical marijuana use and the use or misuse
											of opioids for specific types of pain, and also its possible role for treatment of opioid use disorder. Read
											more in our <em><a href="/node/21190/">Marijuana Research Report</a></em>.
										</p>
							</div>

							<h2>
								What are cannabinoids?
							</h2>

							<p>
								Cannabinoids are chemicals related to <em>delta-9-tetrahydrocannabinol</em> (THC), marijuana&rsquo;s main
								mind-altering ingredient that makes people &quot;high.&quot; The marijuana plant contains more than 100
								cannabinoids. Scientists as well as illegal manufacturers have produced many cannabinoids in the lab. Some of
								these cannabinoids are extremely powerful and have led to serious health effects when misused. Read more in our
								<a href="/drugs-abuse/synthetic-cannabinoids-k2spice"><em>Synthetic Cannabinoids (K2/Spice) DrugFacts</em></a>.
							</p>

							<p>
								The body also produces its own cannabinoid chemicals. They play a role in regulating pleasure, memory,
								thinking, concentration, body movement, awareness of time, appetite, pain, and the senses (taste, touch, smell,
								hearing, and sight).
							</p>

							<div>
								<h3>
									Are People with Health- and Age-Related Problems More Vulnerable to Marijuana&rsquo;s Risks?
								</h3>

								<p>
									State-approved medicinal use of marijuana is a fairly new practice. For that reason, marijuana&rsquo;s effects
									on people who are weakened because of age or illness are still relatively unknown. Older people and those
									suffering from diseases such as cancer or AIDS could be more vulnerable to the drug&rsquo;s harmful effects,
									but more research is needed.
								</p>
							</div>

							<h2>
								How might cannabinoids be useful as medicine?
							</h2>

							<p>
								Currently, the two main cannabinoids from the marijuana plant that are of medical interest are THC and
								CBD.&nbsp;
							</p>

							<p>
								THC can increase appetite and reduce nausea. THC may also decrease pain, inflammation (swelling and redness),
								and muscle control problems.Unlike THC, CBD is a cannabinoid that doesn&#39;t make people &quot;high.&quot;
								These drugs aren&#39;t popular for recreational use because they aren&#39;t intoxicating. It may be useful in
								reducing pain and inflammation, controlling epileptic seizures, and possibly even treating mental illness and
								addictions. Many researchers, including those funded by the National Institutes of Health (NIH), are continuing
								to explore the possible uses of THC, CBD, and other cannabinoids for medical treatment.
							</p>



							<p>
								For instance, recent animal studies have shown that marijuana extracts may help kill certain cancer cells and
								reduce the size of others. Evidence from one cell culture study with rodents suggests that purified extracts
								from whole-plant marijuana can slow the growth of cancer cells from one of the most serious types of brain
								tumors. Research in mice showed that treatment with purified extracts of THC and CBD, when used with radiation,
								increased the cancer-killing effects of the radiation.<a href="#references"><sup>10</sup></a>

								<p>
									Scientists are also conducting preclinical and clinical trials with marijuana and its extracts to treat
									symptoms of illness and other conditions, such as:
								</p>

								<ul>
									<li>
										diseases that affect the immune system, including:
										<ul>
											<li>
												HIV/AIDS
											</li>
											<li>
												multiple sclerosis (MS), which causes gradual loss of muscle control
											</li>
										</ul>
									</li>
									<li>
										inflammation
									</li>
									<li>
										pain
									</li>
									<li>
										seizures
									</li>
									<li>
										substance use disorders
									</li>
									<li>
										mental disorders
									</li>
								</ul>
						</v-card-text>
					</v-flex>

				</v-card>

			</v-container>
		</v-dialog>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				dialog: false
			}
		}
	}
</script>

<style scoped>
	.aurtor {
		color: #78B821
	}

	.aurtor:hover {
		color: #78B821
	}

	.article-img {
	width: 100%;
	height: 250px;
	transition: all 0.2s ease-out;
    object-fit: cover;

	}

	.article-img:hover {
		-webkit-transform: scale(1.05);
		-ms-transform: scale(1.05);
		transform: scale(1.05);
		transition: all 0.2s ease;
		cursor: pointer;
	}

	.article-title {
		color: #707070;
		cursor: pointer;
		border-left: solid 2px #78b821;
		padding-left: 5px;
	}

	.article-main-title {
		border-left: 3px solid #78B821;
		padding-left: 15px;
	}

	a {
		color: none !important;
	}

	.img-box {
		overflow: hidden;
		transition: all 0.2s ease-out;
		box-shadow: -15px 10px 30px -10px #00000099;
		height: 95%;
	}
</style>