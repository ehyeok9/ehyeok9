```Java
public record Developer(
    String summary,
    String[] profile,
    String[] interestedIn,
    Contact contact
) {
    public record Contact(
        String email,
        String linkedIn
    ) {}

    public static Developer hyeokgyuLee() {
        return new Developer(
            "Who strives to validate the process through outcomes.",
            new String[]{
                "Bachelor's Degree in Computer Science at KMU (19.03 ~ 25.02)",
                "Research Intern at STAIRS Lab, UCI (23.06 ~ 23.08)",
                "Backend Developer @ Gausslab Corp. (24.09 ~ 24.11)",
                "Software Engineer @ Meritz Fire & Marine Insurance Co., Ltd. (24.12 ~ ing)"
            },
            new String[]{"Spring Framework/Boot", "DevOps", "Workout"},
            new Contact("ehyeok9@gmail.com", "www.linkedin.com/in/e-hyeok9")
        );
    }
}
```
