# teacherWebApp

This is a web application designed to help teachers and students by harnessing the power of AI.

## TODO:

- Save to pdf
- Speak to dad to ask if necessary. Also how I should get to teachers, and if I should avoid reaching out to districts.
- Have activities tab, to better explain concepts
- Change Teacher helper to menu, and make the second one bigger, bolder, and have logo
- Change purple color to lilac

## Potential Features:

    Lesson Plan Generator:
        Teachers can input a topic, grade level, and duration.
        The app uses ChatGPT to generate a comprehensive lesson plan, including objectives, materials, activities, and assessments.

    Student Feedback Assistant:
        Teachers can input student assignments or performance metrics.
        The app provides constructive feedback and suggestions for improvement, tailored to each student.

    Quiz and Test Creator:
        Generate quizzes and tests based on specified topics and difficulty levels.
        Include multiple-choice, true/false, and short answer questions.

    Classroom Activity Suggestions:
        Provide interactive and engaging activity ideas based on the subject and grade level.
        Offer variations for different learning styles and classroom setups.

    Homework Help Desk:
        Allow students to ask questions or input homework problems.
        The app uses ChatGPT to provide step-by-step explanations and answers.

    Educational Content Summarizer:
        Summarize articles, textbooks, or any educational content.
        Provide concise summaries that highlight key points and concepts.

    Professional Development Resource:
        Curate articles, research papers, and tips for teachers’ professional growth.
        Use ChatGPT to generate summaries or action plans based on the content.

## Docker:

"docker-compose up --build": Run all the containers
"docker run -it -p 4200:4200 -v ${PWD}:/usr/src/app angular-app": Run the docker container with this command

## Angular:

"ng new frontend
cd frontend
ng generate service api
ng generate component lesson-plan-generator
ng generate component quiz-generator": Code to set up the angular project

### Setting up SSL certs:

- "certbot certonly --webroot -w /usr/local/lsws/Example/html -d webexpansions.com -d www.webexpansions.com -d teach.webexpansions.com" use this to add ssl certificate
- Make sure you correctly spell the certificate names above

## Code:

"uvicorn main:app --reload": Start your FastAPI server
"ng serve": Run your angular development server
"chmod +x myscript.sh": Make file runnable
