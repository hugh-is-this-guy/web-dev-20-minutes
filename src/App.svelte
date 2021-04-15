<script>
	export let name;
</script>

<main>
	<section>
		<h1>Hello <span>World</span> {name}!</h1>

		<h2>For this leanring session you will need:</h2>

		<p>
			A relatively up to date version of osx
			<a href="https://www.apple.com/macos/how-to-upgrade/" target="_blank">which you can get here</a>
		</p>

		<p>
			Brew - we install this thing as it helps us then install the other stuff we need.
			<a href="https://brew.sh" target="_blank">You can find instructions right over here</a>
		</p>

		<p>
			xcode-select installed by running <code>xcode-select --install</code>. This is some Apple crap you'll need to run some stuff.
			<a href="https://macpaw.com/how-to/install-command-line-tools" target="_blank">If you'll walk right this way you can find information just over here</a>
		</p>
	</section>

	<section>
		<h3>Alright, that's the boring stuff over. Now! Let's get this flipping thing online!</h3>

		<p>
			We're going to install <em>node</em> using our new friend <em>brew</em>. In your terminal run <code>brew install node</code> and cross your fingers / press your thumbs
		</p>

		<p>
			We're <span>lazy</span> wicked smart so we're going to use a template for our website. We'll get it by running <code>npx degit sveltejs/template learning-session</code>
		</p>

		<p>
			The template we just downloaded needs some things installed in order to run. We'll go into our template by running <code>cd learning-session</code>, and install these things by running <code>npm i</code>
		</p>
	</section>

	<section>

		<h3>We have ourselves a website!</h3>

		<p>
			We're going to run <code>npm run dev</code>, open our web browsers (Chrome or safari or whatever you fancy), and visit <a href="http://localhost:5000/" target="_blank">localhost:5000</a>
		</p>

		<p>
			Beautiful isn't it? Let's get this mother flipping thing online. Signup for a <a href="https://github.com/join">GitHub account</a> - don't worry, it won't cost you a penny. Try to pick a creative username, but no pressure! You can change it later. It took me three goes to get my excellent username <a href="https://github.com/hugh-is-this-guy" target="_blank">hugh-is-this-guy<a>.
		</p>

		<p>
			Create a <a href="https://github.com/new" target="_blank">new repository</a>. A repository is what we call folders we keep our code in. We call them that so people think we're smart. Give it a name - whatever you want. How about Jimbles? Click <em>Create repository</em>
		</p>

		<p>
			So we've got this empty repository just sitting there on GitHub, let's push our code up there. Copy and paste the code under <em>...or push an existing repository from the command line</em>
		</p>

		<p>
			Alright, our template now lives on GitHub. You can now go to <a href="https://github.com/" target="_blank">GitHub</a> and see it all sitting there nicely. What a bloody world eh? LAST STEP! We need someone to take our code, and instead of just storing it, we need them to <em>serve</em> it to us as an actual, real life website.
		</p>

		<p>
			There's literally hundreds of places we can get to serve our websites for us, and today we're going to use one called <em>Vercel</em> because it's got the coolest name. Go to <a href="https://vercel.com/signup" target="_blank">https://vercel.com/signup</a> and log in with your shiny new GitHub account.
		</p>

		<p>
			Make a new project! Either find the button that says <em>New Project</em>, or if you're feeling lazy, just click on <a href="https://vercel.com/new" target="_blank">this link</a>. We're all friends here, I'm not gunna judge you.
		</p>

		<p>
			Vercel should show you a list of your repositories, you just click on it and you're good to go. You select your personal account, as it's free then (I know right??). Check that the name is right, and that Vercel has worked out it's a Svetle site. Click Deploy...
		</p>

		<p>
			Click the visit button! You can do it! IT'S THE LAST STEP! OH MY GOD THERE IT IS! HOLY COW WE ACTUALLY DID IT! (Comiserations if you didn't make it this far. Give me a shout on slack and we'll sort it out.)
		</p>
	</section>

	<section>
		<h3>Holy smokes that was easy. Now let's make some changes?</h3>

		<p>
			Ok fine that wasn't the last step. But we literally just followed a few (alright, <em>quite</em> a few) steps and we have a website out on the actual internet. If you ask me that's pretty rad. Now, let's make some changes to our code. (You may want to download a fancy looking code editor to make your changes. I personally like <a>this one</a>, as again, it has a cool name.)
		</p>

		<p>
			Made your changes? Alright in the terminal we're going to run <code>git add .</code> <code>git commit -m 'This web dev thing is a piece of cake'</code> and finally <code>git push</code>.
		</p>

		<p>
			BOOM. We're done. You're officially a web developer. Please submit your CVs to hugh@blinkist.com and I'll go retire on the recruitment bonuses. Now get out of here you crazy kids, go build yourself some websites to your heart's content
		</p>
	</section>

	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	main {
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	section {
		padding-bottom: 1em;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		text-align: center;
		font-size: 4em;
		font-weight: 100;
	}

	span {
		text-decoration: line-through;
	}

	p {
		padding-bottom: 16px;
	}

	em {
		font-weight: bold;
		font-style: normal;
	}

	code {
		color: #000;
    background: #f3f3f3;
		padding: 3px 8px;
		border-radius: 4px;
	}

	@media (min-width: 640px) {
		main {
			max-width: 820px;
		}
	}
</style>
