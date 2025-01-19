<script>
  const challenges = [
    { month: 'January', items: [{ icon: '🧑🏻‍💻🎨', name: 'Genuary', link: 'https://genuary.art/' }] },
    { month: 'February', items: [{ icon: '🎨', name: 'Februllage', link: 'https://missprinted.no/februllage/' }] },
    { month: 'March', items: [
      { icon: '🎨', name: 'March of Robots', link: 'https://www.instagram.com/marchofrobots/' },
      { icon: '🎨', name: 'March Meet the Maker', link: 'https://www.marchmeetthemaker.com' }
    ]},
    { month: 'April', items: [{ icon: '🎨', name: 'April Art Challenge', link: 'https://www.instagram.com/explore/tags/aprilartchallenge/' }] },
    { month: 'May', items: [
      { icon: '🧑🏻‍💻🎨', name: 'Mayterials', link: 'https://x.com/mayterials' },
      { icon: '🎨', name: 'Mermay', link: 'https://www.mermay.com/' },
      { icon: '🎨', name: 'May Sketch a Day', link: 'https://www.instagram.com/explore/tags/maysketchaday/' }
    ]},
    { month: 'June', items: [
      { icon: '🎨', name: 'Junetoon', link: 'https://haroldgeorge.com/junetoon' },
      { icon: '🎨', name: 'Junefae', link: 'https://brushwarriors.com/junefae-art-challenge/' }
    ]},
    { month: 'July', items: [{ icon: '🎨', name: 'July Drawing Challenge', link: 'https://www.instagram.com/explore/tags/julydrawingchallenge/' }] },
    { month: 'October', items: [
      { icon: '🧑🏻‍💻', name: 'Hacktoberfest', link: 'https://hacktoberfest.com/' },
      { icon: '🎨', name: 'Inktober', link: 'https://inktober.com/' },
      { icon: '🧑🏻‍💻🎨', name: 'Hooptober', link: 'https://letterboxd.com/cinemonster/' },
      { icon: '🧑🏻‍💻🎨', name: 'Swordtober', link: 'https://www.reddit.com/r/Swordtember/' }
    ]},
    { month: 'November', items: [{ icon: '🧑🏻‍💻🎨', name: 'Nodevember', link: 'https://nodevember.io/' }] },
    { month: 'December', items: [{ icon: '🧑🏻‍💻', name: 'Advent of Code', link: 'https://adventofcode.com/' }] },
    { month: 'Partial Year', items: [
      { icon: '🧑🏻‍💻🎨', name: '36 Days of type', link: 'https://www.36daysoftype.com/' },
      { icon: '🧑🏻‍💻', name: '100 Days of Code', link: 'https://www.100daysofcode.com/' },
      { icon: '🧑🏻‍💻', name: '100 Days of SwiftUI', link: 'https://www.hackingwithswift.com/100/swiftui' }
    ]},
    { month: 'All Year', items: [{ icon: '', name: 'Buzzwordathon', link: 'https://www.booksandlala.com/blog/buzzwordathon-2024' }] }
  ];
</script>

<main>
  <h1>Yallenges</h1>
  <p>List of all the yearly challenges I have found that happen every year.</p>
  <ul>
    {#each challenges as { month, items }}
      <li>
        <h2>{month}</h2>
        <ul>
          {#each items as { icon, name, link }}
            <li>
              <a href={link} target="_blank">{icon} {name}</a>
            </li>
          {/each}
        </ul>
      </li>
    {/each}
  </ul>
</main>

<style>
  main {
    font-family: Arial, sans-serif;
    padding: 2rem;
  }
  h1 {
    text-align: center;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    margin: 0.5rem 0;
  }
  a {
    text-decoration: none;
    color: #007acc;
  }
  a:hover {
    text-decoration: underline;
  }
</style>