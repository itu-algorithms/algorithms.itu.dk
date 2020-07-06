# ITU Algorithms group web pages

The [live version](http://itu-algorithms.github.io) is visible to the world.

## Usage

Simple updates (such as a news item or event) can be done by adding single text files in Markdown format to the git repository.
(If you want to do more serious modifications to the blog, it’s probably a good idea to clone the repo, make local changes, add them, commit, and push.)

### Adding posts and events

Every event and news item is a separate text file in the `_posts` folder.
The file name starts with the date of hte news item of event, as `YYYY-MM-DD-whatever.md`, for instance `2015-02-22-talk-by-turing.md`.
Each text file must begin with a title between two lines of three dashes.
A minimal news item looks like this:

    ---
    title: New group language policy
    ---
    The group has adapted German as the default language for talks
    and social interaction.

Posts are in Markdown format, so you can do something like this:

    ---
    title: New group language policy
    ---
    The group has adapted *German* as the default language for talks
    and informal interaction.


Mathjax is activated in all posts, so you can do something like this:

    ---
    title: Group abandons circle constant
    ---
    As a matter of group policy, the algorithm group will henceforth
    use the circle constant \\(\tau\\) instead of \\(pi\\).
    For instance, \\(A = \pi r^2\\) will be given as
    \\( A = \frac{1}{2} \tau r^2\\).

(The Markdown preprocessor and Mathjax interact in funky and ill-defined ways. There’s not much one can do about that other than trying various backslashes to escape backslashes and underscore.)

A post that is not a news item needs to be categorised as an event.
Posts may have speaker, place, and time fields set in the frontmatter.
A typical event looks like this:

    ---
    title: Approximate Range Emptiness in Constant Time and Optimal Space
    category: events
    time: 11–12
    place: 3A11
    speaker: Rasmus Pagh
    ---
    Joint work with Mayank Goswami, Allan Grønlund, and Kasper Green Larsen

    Presented at SODA 2015

    Abstract: This paper studies the ε-approximate range emptiness problem, where the task is to represent a set S of n points from \\(\\{0, \ldots , U − 1\\}\\)
    and answer emptiness queries of the form “ \\([a; b] \cap S\neq \emptyset ?\\) ”

### Members

The database of group members is another text file in YML format at `_data/members.yml`.

## License

[MIT](http://opensource.org/licenses/MIT)
