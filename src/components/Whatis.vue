<template>
    <!-- Information Sections -->
    <div class="space-y-8 text-white">
        <!-- Dyslexia Section -->
        <section
            class="flex flex-col md:flex-row gap-8 items-center max-w-6xl 2xl:max-w-none ml-auto rounded-l-2xl bg-secondary p-10">
            <div class="w-full md:w-1/3">
                <img src="../../src/assets/girl-reading.webp" alt="What is Dyslexia?"
                    class="w-full h-[400px] object-cover rounded-lg shadow-lg" title="What is Dyslexia?">
            </div>

            <div class="w-full md:w-2/3 space-y-4">
                <h3 class="text-3xl uppercase font-bold">What is Dyslexia?</h3>

                <p class="mt-4">The Devon Local Authority has settled on the following definition of Dyslexia:</p>
                <blockquote class="pl-4 border-l-4 border-primary italic">
                    "Dyslexia is evident when accurate and fluent reading and or spelling develops very
                    incompletely or with great difficulty. This focuses on literacy learning at the 'word level' and
                    implies that the problem is severe and persistent despite appropriate learning opportunities"
                    (British Psychological Society 1999)
                </blockquote>

                <p>The SpLD Assessment and Standards Committee (SASC) adopted a new updated
                    definition of dyslexia, which the main professional bodies have also adopted (BDA,
                    PATOSS & Dyslexia Guild). March 2025:</p>
                <blockquote class="pl-4 border-l-4 border-primary italic">
                    <span class="underline">The Delphi definition of dyslexia.</span>
                    <br>
                    <br>
                    <span class="underline">Nature</span>
                    <br>
                    <span class="italic text-sm">"The nature and developmental trajectory of dyslexia depend on multiple genetic and
                    environmental influences."</span>
                    <br>
                    <br>
                    <span class="underline">Manifestation</span>
                    <br>
                    <span class="italic text-sm">"Dyslexia is a set of processing difficulties that affect the acquisition of reading and
                    spelling. The most commonly observed cognitive impairment in dyslexia is a difficulty in
                    phonological processing (i.e. in phonological awareness, phonological processing
                    speed or phonological memory). However, phonological difficulties do not fully explain
                    the variability that is observed. Working memory, processing speed and orthographic
                    skills can contribute to the impact of dyslexia."</span>

                    <br>
                    <br>
                    <span class="underline">Impact</span>
                    <br>
                    <span class="italic text-sm">"In dyslexia, some or all aspects of literacy attainment are weak in relation to age,
                    standard teaching and instruction, and level of other attainments. Across languages
                    and age groups, difficulties in reading fluency and spelling are a key marker of dyslexia.
                    Variance and co-occurrence
                    Dyslexic difficulties exist on a continuum and can be experienced to various degrees of
                    severity. Dyslexia can affect the acquisition of other skills, such as mathematics,
                    reading comprehension or learning another language. Dyslexia frequently co-occurs
                    with one or more other developmental difficulties, including developmental language
                    disorder, dyscalculia, ADHD, and developmental coordination disorder.""</span>

                    <br>
                    <br>
                    <span class="italic text-xs">Carroll, J., Holden, C., Kirby, P., Snowling, M. J., & Thompson, P.A. (2025) Journal of Child
                    Psychology and Psychiatry.</span>
                </blockquote>

                <p>If you would like to know more about Dyslexia or need help understanding either of these
                    definitions,
                    I am more than happy to help and am always contactable via email.</p>

                <router-link to="/assessments" class="primary-button">
                    Dyslexia assessments
                </router-link>
            </div>
        </section>
        s
        <!-- Qualifications Section -->
        <section
            class="flex flex-col md:flex-row gap-8 items-center max-w-6xl 2xl:max-w-none ml-auto rounded-l-2xl bg-secondary p-10">
            <div class="w-full md:w-1/3">
                <img src="../../src/assets/numbers.webp" alt="Dyslexia Tutor Qualifications"
                    class="w-full h-[400px] object-cover rounded-lg shadow-lg" title="Dyslexia Tutor Qualifications">
            </div>

            <div class="w-full md:w-2/3 space-y-4">
                <h3 class="text-3xl uppercase font-bold">What qualifications should a dyslexia tutor or assessor
                    have?</h3>

                <p class="mt-4">
                    A specialist dyslexia tutor should have a level 5 qualification which will provide them with the
                    title of
                    <strong class="italic">Dyslexia Specialist Tutor</strong>. A level 5 course is needed for anyone
                    wanting to work privately as a dyslexia tutor or to work in a role designated for a dyslexia
                    specialist.
                </p>

                <p>
                    Dyslexia specialists who are qualified to MA level (level 7) will have done further training
                    past level 5 in
                    <strong class="italic">Psychometric Testing and assessment</strong> and are formally qualified
                    to assess for Dyslexia.
                </p>

                <p>
                    As a parent looking for a 1:1 dyslexia tutor, you should ensure your tutor has a
                    <strong class="italic underline decoration-primary decoration-2">level 5 qualification</strong>
                    and for assessments, a
                    <strong class="italic underline decoration-primary decoration-2">level 7 qualification</strong>.
                    A level 7 assessor should also hold an
                    <strong class="italic">APC (assessment practising certificate)</strong>, meaning the report
                    provided on the results can be used for the Disabled Student's Allowance (DSA).
                </p>

                <div class="bg-white/5 p-6 rounded-lg border border-primary/20 backdrop-blur-sm mt-8">
                    <h3 class="text-xl font-semibold mb-4">My Qualifications</h3>
                    <ul class="list-disc pl-6 space-y-2">
                        <li>B.Ed</li>
                        <li>PG Cert (SpLD - dyslexia)</li>
                        <li>Level 5 dyscalculia</li>
                        <li>APC</li>
                        <li>AMBDA</li>
                        <li>DBS checked</li>
                    </ul>
                </div>

                <router-link to="/#qualifications" class="primary-button" @click="scrollToQualifications">
                    My qualifications
                </router-link>
            </div>
        </section>

        <!-- Help at Home Section -->
        <section
            class="flex flex-col md:flex-row gap-8 items-center max-w-6xl 2xl:max-w-none mr-auto rounded-r-2xl bg-secondary p-10">

            <div class="w-full md:w-2/3 space-y-4">
                <h3 class="text-3xl uppercase font-bold">How can I help my child at home?</h3>

                <ul class="space-y-4 list-disc pl-6">
                    <li>Help your child to develop strategies that will help them in the classroom</li>
                    <li>Work with the school to find the best ways of supporting your child</li>
                    <li>Encourage them to talk about their difficulties and to let others know</li>
                    <li>Give lots of praise when they achieve something that they are proud of</li>
                    <li>Encourage them to take up activities that they enjoy or feel good about</li>
                    <li>Avoid being negative or comparing them to someone who is successful</li>
                    <li>Avoid talking to others about their difficulties, especially in their hearing</li>
                </ul>

                <p class="mt-6">If you need guidance on implementing any of these strategies or would like more
                    specific advice for your child's situation, please don't hesitate to get in touch.</p>
            </div>

            <div class="w-full md:w-1/3">
                <img src="../../src/assets/boy-reading.webp" alt="How can I help my child?"
                    class="w-full h-[400px] object-cover rounded-lg shadow-lg" title="How can I help my child?">
            </div>
        </section>

        <!-- Working Memory Section -->
        <section
            class="flex flex-col md:flex-row gap-8 items-center max-w-6xl 2xl:max-w-none ml-auto rounded-l-2xl bg-secondary p-10">
            <div class="w-full md:w-1/3">
                <img src="../../src/assets/girl-reading.webp" alt="Supporting Working Memory"
                    class="w-full h-[400px] object-cover rounded-lg shadow-lg" title="Supporting Working Memory">
            </div>

            <div class="w-full md:w-2/3 space-y-4">
                <h3 class="text-3xl uppercase font-bold">How to support the working memory</h3>

                <ul class="space-y-4 list-disc pl-6">
                    <li>Use simple language and don't speak too fast so as to avoid over loading your child with
                        information</li>
                    <li>Give instructions one at a time and ensure each instruction is grasped before continuing
                    </li>
                    <li>Find out what your child is struggling with, and be prepared to recognise when it is
                        necessary to repeat instruction etc</li>
                </ul>

                <p class="mt-6">If you would like more specific strategies for supporting your child's working
                    memory, please get in touch for personalized advice.</p>

                <router-link to="/contact" class="primary-button">
                    Contact me
                </router-link>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    methods: {
        scrollToQualifications() {
            setTimeout(() => {
                const element = document.getElementById('qualifications');
                if (element) {
                    element.scrollIntoView({ behavior: 'smooth' });
                }
            }, 100); // 100ms delay to ensure route change completes
        }
    }
}
</script>