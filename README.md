Hi, I'm Melanati Medha Sree, a passionate and driven Computer Science Engineer with a strong foundation in programming and problem-solving. I'm excited to leverage my skills and knowledge to contribute to innovative projects and collaborate with like-minded individuals.

With a solid educational background from Ravindra College of Engineering, I've developed expertise in programming languages (C, Java, DSA), web development (HTML, CSS, JavaScript), and database management. My experience with projects like Online Banking System and Text Classification with TensorFlow has honed my skills in software development and artificial intelligence.





public class Resume {
    private String name;
    private Contact contact;
    private String objective;
    private String[] skills;
    private Experience[] experiences;
    private Education education;
    private String[] certifications;

    public Resume() {
        this.name = "Melanati Medha Sree";
        this.contact = new Contact("8317632985", "medhasree45@gmail.com");
        this.objective = "Dynamic Computer Science Engineer seeking a challenging role";
        this.skills = new String[] {
            "Programming: C, Java, DSA",
            "Web Technology: HTML, CSS, JavaScript, SQL",
            "Soft Skills: Communication, Leadership, Time Management"
        };
        this.experiences = new Experience[] {
            new Experience("Online Banking System", "Java, DBMS"),
            new Experience("Text Classification with TensorFlow", "Python"),
            new Experience("Virtual Internships", "Java, AI, Web Development")
        };
        this.education = new Education("Ravindra College of Engineering", "Computer Science & Engineering", "78.66%", "2021-2025");
        this.certifications = new String[] {
            "DSA",
            "Java Full Stack",
            "Data Engineering",
            "Cyber Security",
            "App Development",
            "Soft Skills",
            "IBM Cloud Computing"
        };
    }

    public static void main(String[] args) {
        Resume resume = new Resume();
        System.out.println("Name: " + resume.name);
        System.out.println("Contact: " + resume.contact.phone + ", " + resume.contact.email);
        System.out.println("Objective: " + resume.objective);
        System.out.println("Skills: ");
        for (String skill : resume.skills) {
            System.out.println(skill);
        }
        System.out.println("Experiences: ");
        for (Experience experience : resume.experiences) {
            System.out.println(experience.project + ": " + experience.technology);
        }
        System.out.println("Education: ");
        System.out.println(resume.education.institution + ", " + resume.education.degree + ", " + resume.education.percentage + ", " + resume.education.duration);
        System.out.println("Certifications: ");
        for (String certification : resume.certifications) {
            System.out.println(certification);
        }
    }
}

class Contact {
    String phone;
    String email;

    public Contact(String phone, String email) {
        this.phone = phone;
        this.email = email;
    }
}

class Experience {
    String project;
    String technology;

    public Experience(String project, String technology) {
        this.project = project;
        this.technology = technology;
    }
}

class Education {
    String institution;
    String degree;
    String percentage;
    String duration;

    public Education(String institution, String degree, String percentage, String duration) {
        this.institution = institution;
        this.degree = degree;
        this.percentage = percentage;
        this.duration = duration;
    }
}


**OUTPUT:**

Name: Melanati Medha Sree
Contact: 8317632985, medhasree45@gmail.com
Objective: Dynamic Computer Science Engineer seeking a challenging role
Skills: 
Programming: C, Java, DSA
Web Technology: HTML, CSS, JavaScript, SQL
Soft Skills: Communication, Leadership, Time Management
Experiences: 
Online Banking System: Java, DBMS
Text Classification with TensorFlow: Python
Virtual Internships: Java, AI, Web Development
Education: 
Ravindra College of Engineering, Computer Science & Engineering, 78.66%, 2021-2025
Certifications: 
DSA
Java Full Stack
Data Engineering
Cyber Security
App Development
Soft Skills
IBM Cloud Computing
