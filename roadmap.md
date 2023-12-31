# Roadmap for the project

*This is less of a roadmap and more of a list of things I'd like to get to at some point. There are no timeframes and no pressure to do any of it at all.*

**Content**: Right now, there isn't much content on the site at all, as I'm focused on building out the infrastructure and functionality. For example, I'm working on updating the existing page metadata (i.e. page titles, descriptions, and tags). I'm also mostly adding content just to see how it looks. Once I'm reasonably happy with the look of the pages I'll create a template that can be applied to all pages so that any content I do add looks similar across the site. Once I'm happy with the general look and feel, I'll start adding information from my notes.

**Newsletter**: I want to build an [automated newsletter](https://medium.com/geekculture/how-to-create-an-automated-newsletter-for-free-7522c5646b50) where I can dump items of interest during the week, which get posted out to a mailing list automatically. I have no idea how to do this, other than suspecting it has something to do with [Github Actions](https://support.github.com/features/actions).

**Search**: Because this site is built with a static site generator (i.e. no database or PHP...just plain HTML) there's no search function that's easy to integrate. Because I want this to be a dictionary as well as a programme of study, search is probably important to include. I have no idea how to do this.

**Analytics**: I'd like to include an open-source version of Google Analytics on the site. This is complicated because Pages only hosts static web content and doesn't support any server-side processing. So I'd need to host the software on another server, which means it's possible but complicated. [Offen](https://www.offen.dev/) looks like a good option.

**SEO tags**: I've started adding metadata to the pages generated on the site, but the *SEO tag* plugin gives more granular options for adding metadata to the site. This helps with search and discoverability.

**Search engines**: Submit the site to other search engines. I've done Google because I know that process relatively well. I also want to do Bing and Yandex. This is a simple process that shouldn't take long.

**Library**: I want to add a library of sorts. Or maybe an annotated bibliography. Basically, a way to post summaries and reviews of books and other long-form content that I'm working through. I'm considering a shared Zotero library. Something [like this](https://www.zotero.org/groups/2431045/ai_in_healthcare/library). This would mean that I can keep using Zotero to manage my resources, while also sharing annotations.

**CSS**: One of the reasons I wanted to create this site as a project is that it would give me a reason to tinker with HTML and CSS again. Before content management systems like WordPress, I used to build websites by writing the raw HTML and CSS. I really enjoyed the process and thought I could eventually start styling the site beyond the basic themes that Github Pages supports. This is an aesthetic feature though, so is pretty low on the list.

**Translation**: Because the site is hosted in Github and the content is open-access, it means that anyone can modify this content and create new versions. It might be nice if someone wanted to create translations of the English version of the project. No pressure.

---

# Completed

**Blog** (29 Dec 2023: I feel like the site needs a News section, where I can share progress updates on technical features that get included (for example, documenting the process of building a site like this), content updates, and so on. The process for creating a blogging feature in Jekyll seems fairly well-documented, so it's likely that this will happen sooner than other features.