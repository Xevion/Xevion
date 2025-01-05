<p align="center">
  <samp>
    <a href="https://xevion.dev">me</a> .
    <a href="https://undefined.behavio.rs">blog</a> .
    <a href="https://xevion.dev/projects">projects</a> .
    <a href="https://status.xevion.dev">status</a>
  </samp>
</p>

```rust
use std::env;
use std::collections::HashMap;
use rand::seq::SliceRandom;

use Life::Interests::Technology::{
    Languages::{Go, Rust},
    Fields::{GameHacking, WebDevelopment},
    Infrastructure::{Unraid, Docker},
};
use Life::Mental::Traits::{Diagnosed::ADHD, Undiagnosed::Autism};
use Life::Interests::Arts::{Photography, DigitalArt::AIArt};
use Life::Interests::Gaming::Simulation::{Factorio, RimWorld};

impl Human {
    fn me(username: &str) -> Human {
        let middle_name = vec![env::var("MIDDLE_NAME").unwrap_or_default().as_str(), "C", ""].choose(&mut rand::thread_rng()).unwrap_or(&"");
        let name = format!("Ryan {} W.", middle_name);

        let endpoints = std::collections::HashMap::from([
            ("discord", ".xevion"),
            ("email", "xevion@xevion.dev"),
        ]);

        Human {
            name,
            pronouns: vec!["he", "they"],
            occupation: Life::Occupations::Student::University.pull(),
            description: "
                A full-stack software engineer navigating their way through the industry.
                With an attention to detail, I enjoy building projects that are elegant, robust, and impactful.
                Although I specialize in Web Development, my skill set is extensive, and I'm confident in my ability to learn anything.",
            recent_projects: vec![
                "https://github.com/acmutsa/Portal",
                "https://github.com/Xevion/rdap",
                "https://github.com/Xevion/grain",
            ],
            endpoints,
        }
    }
}
```
