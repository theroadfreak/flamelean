<template>
	<section class="bg-e6e6e6">
		<div class="container py-5">
			<h5 class="text-7C7C7C mb-5">Scientific References:</h5>
			<div
				class="col-12 mb-lg-5 row d-flex align-items-center justify-content-center"
			>
				<div
					v-for="(logo, i) in logos"
					:key="i"
					class="col-6 col-sm-5 col-lg-3"
				>
					<img
						:src="
							require('../../assets/images/index/scientific-references/' +
								logo.image)
						"
						:alt="logo.alt"
						class="col-12"
					/>
				</div>

				<div class="small text-center fw-lighter pt-4">
					FlameLean is not endorsed by, sponsored by, or
					<br class="d-none d-sm-flex" />
					affiliated with any of these organizations.
					<br class="d-none d-sm-flex" />
					Jessica is a pen name in this pitch page.
				</div>
			</div>
			<div class="row">
				<div
					v-for="(reference, i) in scientificReferences"
					:key="i"
					class="col-12 col-lg-6 mb-3"
				>
					<p class="small custom-wrap">{{ reference }}</p>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: "ScientificReferencesSection",
	data() {
		return {
			logos: [
				{
					image: "harvard-logo.svg",
					alt: "Harvard logo",
				},
				{
					image: "new-york-obesity-research-center-logo.svg",
					alt: "New York Obesity Research Center logo",
				},
				{
					image: "imperial-college-healthcare-logo.svg",
					alt: "Imperial College Healthcare logo",
				},
				{
					image: "oxford-logo.svg",
					alt: "Oxford logo",
				},
			],
			scientificReferences: [
				"1. Gammone MA, D'Orazio N. Anti-obesity activity of the marine carotenoid fucoxanthin. Mar Drugs. 2015;13(4):2196-2214. Published 2015 Apr 13. doi:10.3390/md13042196",
				"7. Maeda H, Hosokawa M, Sashima T, Funayama K, Miyashita K. Fucoxanthin from edible seaweed, Undaria pinnatifida, shows antiobesity effect through UCP1 expression in white adipose tissues. Biochem Biophys Res Commun. 2005;332(2):392-397. doi:10.1016/j.bbrc.2005.05.002",
				"2. Arif Icer M, Acar Tek N. Effects of Red Pepper, Ginger, and Turmeric on Energy Metabolism: Review of Current Knowledge. Altern Ther Health Med. 2021;AT6422.",
				"8. Zou T, Li S, Wang B, Wang Z, Liu Y, You J. Curcumin improves insulin sensitivity and increases energy expenditure in high-fat-diet-induced obesity associated with activation of FNDC5/irisin. Nutrition. 2021;90:111263. doi:10.1016/j.nut.2021.111263",
				"3. Ngondi JL, Etoundi BC, Nyangono CB, Mbofung CM, Oben JE. IGOB131, a novel seed extract of the plant Irvingia gabonensis, significantly reduces body weight and improves metabolic parameters in overweight humans in a randomized double-blind placebo controlled investigation. Lipids Health Dis. 2009;8:7. Published 2009 Mar 2. doi:10.1186/1476-511X-8-7",
				"9. Oben JE, Ngondi JL, Blum K. Inhibition of Irvingia gabonensis seed extract (OB131) on adipogenesis as mediated via down regulation of the PPARgamma and leptin genes and up-regulation of the adiponectin gene. Lipids Health Dis. 2008;7:44. Published 2008 Nov 13. doi:10.1186/1476-511X-7-44",
				"4. Burke AC, Sutherland BG, Telford DE, et al. Intervention with citrus flavonoids reverses obesity and improves metabolic syndrome and atherosclerosis in obesity. J Lipid Res. 2018;59(9):1714-1728. doi:10.1194/jlr.M087387",
				"10. Park J, Kim HL, Jung Y, Ahn KS, Kwak HJ, Um JY. Bitter Orange (Citrus aurantium Linné) Improves Obesity by Regulating Adipogenesis and Thermogenesis through AMPK Activation. Nutrients. 2019;11(9):1988. Published 2019 Aug 22. doi:10.3390/nu11091988",
				"5. Waterman C, Rojas-Silva P, Tumer TB, et al. Isothiocyanate-rich Moringa oleifera extract reduces weight gain, insulin resistance, and hepatic gluconeogenesis. Mol Nutr Food Res. 2015;59(6):1013-1024. doi:10.1002/mnfr.201400679",
				"11. Kilany OE, Abdelrazek HMA, Aldayel TS, Abdo S, Mahmoud MMA. Anti-obesity potential of Moringa olifera seed extract and lycopene on high fat diet induced obesity in male Sprauge Dawely rats. Saudi J Biol Sci. 2020;27(10):2733-2746. doi:10.1016/j.sjbs.2020.06.026",
				"6. Mansour MS, Ni YM, Roberts AL, Kelleman M, Roychoudhury A, St-Onge MP. Ginger consumption enhances the thermic effect of food and promotes feelings of satiety without affecting metabolic and hormonal parameters in overweight men: a pilot study. Metabolism. 2012;61(10):1347-1352. doi:10.1016/j.metabol.2012.03.016",
				"12. Wang J, Li D, Wang P, Hu X, Chen F. Ginger prevents obesity through regulation of energy metabolism and activation of browning in high-fat diet-induced obesity. J Nutr Biochem. 2019;70:105-115. doi:10.1016/j.jnutbio.2019.05.001",
				"13. https://www.nbcnews.com/health/health-news/people-diabetes-struggle-find-ozempic-soars-popularity-weight-loss-aid-rcna64916 https://www.forbes.com/sites/ariannajohnson/2022/12/26/what-to-know-about-ozempic/?sh=24e00d9b5adb https://www.nytimes.com/2022/11/22/well/ozempic-diabetes-weight-loss.html https://www.vice.com/en/article/epz93n/ozempic-viral-celebrity-weight-loss-drug https: //variety.com/2022/film/actors/weight-loss-ozempic-semaglutide-hollywood-1235361465/ https://www.nbcnews.com/health/health-news/people-diabetes-struggle-find-ozempic-soars-popularity-weight-loss-aid-rcna64916",
				"14. https://www.buzzfeednews.com/article/anthonyrobledo/celebrities-ozempic-weight-loss-drug-trend-quotes https://www.webmd.com/diet/obesity/news/20221129/the-tiktok-trend-that-triggered-a-diabetes-drug-shortage https://www.forbes.com/sites/ariannajohnson/2022/12/26/what-to-know-about-ozempic/?sh=24e00d9b5adb https://www.singlecare.com/ blog/ozempic-alternatives/ https: //www.womenshealthmag.com /uk /food/weight-loss/a42280255/ozempic-weight-loss-drug-explainer/",
			],
		};
	},
};
</script>

<style scoped>
.bg-e6e6e6 {
	background-color: #e6e6e6;
}

.text-7C7C7C {
	color: #7c7c7c;
}

.text-4D4D4D {
	color: #4d4d4d;
}
.custom-wrap {
	word-wrap: break-word;
}
</style>
