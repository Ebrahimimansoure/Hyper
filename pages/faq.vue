<template>
    <div class="w-full">
        <BreadCrumb/>
        <div class="flex flex-wrap flex-col justify-center max-w-screen-xl m-auto md:px-4 md:py-8 border-b border-gray-400">
            <div class="flex flex-wrap flex-col w-full items-center justify-center">
                <div class="flex flex-wrap w-full items-start justify-center md:justify-between">
                    <!--image of width 1/5 in tablet and large screen and 10/12 in mobile-->
                    <img src="/faq.jpg" alt="Frequently Asked Questions" class="md:rounded-xl w-full md:w-2/5  aspect-16/9 md:aspect-square object-cover">
                    <!--Other content-->
                    <div class="flex flex-wrap flex-col w-10/12 md:w-3/5 md:pl-8 md:pr-4 pl-0 pr-0 py-4">
                        <!--Name with the icon of user-->
                        <h2 class="info-label">
                            Can I share the program details with my friends and classmates? 
                        </h2>
                        <p class="info-content">
                            Absolutely! We encourage participants to spread the word and invite friends who might be interested in joining the program
                        </p>

                        <h2 class="info-label">
                            Will I receive a certificate after completing the free summer school? 
                        </h2>
                        <p class="info-content">
                            Yes, participants who successfully complete the program will receive a certificate of participation.
                        </p>

                        <h2 class="info-label">
                            Is attendance mandatory for all sessions? 
                        </h2>
                        <p class="info-content">
                            While regular attendance is recommended to get the most out of the program, we understand that summer schedules can vary.
                        </p>

                        <h2 class="info-label">
                            Are there any assignments or assessments during the program?
                        </h2>
                        <p class="info-content">
                            While there might be informal assessments to gauge understanding, the focus is on fostering a collaborative and engaging learning environment.
                        </p>

                        <h2 class="info-label">
                            What is the purpose of the free summer school program?
                        </h2>
                        <p class="info-content">
                            The free summer school program aims to provide educational opportunities and enrichment activities for students during the summer break
                        </p>

                        <h2 class="info-label">
                            Will accommodation be provided for participants? 
                        </h2>
                        <p class="info-content">
                            Accommodation is not provided for this program
                        </p>

                        <h2 class="info-label">
                            Is there a dress code for the program? 
                        </h2>
                        <p class="info-content">
                            The dress code is generally casual and comfortable, but there may be specific guidelines for certain activities.
                        </p>

                        <h2 class="info-label">
                            What language will the program be conducted in?
                        </h2>
                        <p class="info-content">
                            The program will be conducted primarily in <strong>English</strong>, with potential translationsin Italian if needed.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.info-label {
    @apply text-xl text-indigo-950;    
}
.info-content {
    @apply text-base text-gray-800 mb-4;
}
</style>

