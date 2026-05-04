/*════════════════════════════════════════════
    Automail Uniformity Styling V1.0.1 by @hoh and @Reina (compiled by @pseudo)
    https://anilist.co/user/pseudo/
    Modular: PARTIALLY (Read Description)
════════════════════════════════════════════*/

/*════════════════════════════════════════════
This snippet has two purposes:
  - Apply universal styling to Hoh (Automail) profile elements (E.G. hide them or change colours)
  - Self-host and apply various Automail togglable features as default implementations (Hollow unliked hearts and list counters)

This is modular IF YOU ALSO SPECIFY THE SAME PROFILE VARIABLES (--foreground and --border-radius) AS I DO.
Otherwise, you'll see no effect for any selectors which use these variables. --color-blue, however, will work.
In addition, if you want to keep some elements which are set to display: none, this probably isn't as modular as you'd like.
════════════════════════════════════════════*/

/*═══ Standardization ═══*/
.hohDownload, 
.hohDismiss { 
    display: none !important; /* Hides the Banner Download and Dismiss buttons */
}
.hohButton { 
    background: rgb(var(--color-blue)) !important;
}
.hohTable,
.hohTable .header,
.hohThemeSwitch,
.hohActive,
.hohDisplayBox {
    background: var(--foreground) !important; /* Makes various elements adhere to my --foreground variable */
}
.activity-feed .details .hohScore {
    border-radius: var(--border-radius) !important; /* Makes the score on profile overview adhere to my --border-radius variable */
}

/*═══ Automail/@Reina's Hollow Unliked Hearts ═══*/
.action.likes .button,
.like-wrap.thread_comment .button {
	color: rgb(var(--color-blue-dim));
}
.action.likes .button:hover,
.like-wrap.thread_comment .button:hover {
	color: rgb(var(--color-blue));
}
.action.likes .button .fa-heart,
.like-wrap.thread_comment .button .fa-heart {
	color: #0000;
	stroke: rgb(var(--color-blue-dim));
	stroke-width: 70;
	font-size: 0.87em;
	padding-bottom: 0.08em;
	padding-top: 0.05em;
}
.action.likes .button .fa-heart:hover,
.like-wrap.thread_comment .button .fa-heart:hover {
	stroke: rgb(var(--color-blue));
}
.action.likes .button.liked,
.like-wrap.thread_comment .button.liked {
	color: rgb(var(--color-red));
}
.action.likes .button.liked:hover,
.like-wrap.thread_comment .button.liked:hover {
	--color-red: 246, 124, 144;
	color: rgb(var(--color-red));
}
.action.likes .button.liked:hover .fa-heart,
.like-wrap.thread_comment .button.liked:hover .fa-heart {
	color: rgb(var(--color-red));
}
.action.likes .button.liked .fa-heart,
.like-wrap.thread_comment .button.liked .fa-heart {
	color: var(--color-red);
	stroke: rgba(0, 0, 0, 0);
	stroke-width: 0;
	font-size: 0.875em;
	padding-bottom: 0;
	padding-top: 0;
}
.action.likes .button.liked .fa-heart:hover,
.like-wrap.thread_comment .button.liked .fa-heart:hover {
	color: rgb(var(--color-red));
}

/*═══ @hoh's/Automail's List Counters ═══*/
.list-wrap {
	counter-reset: listCounter;
}
.medialist.table.compact .entry .title::before, .medialist.table .entry .title::before {
    counter-increment: listCounter;
    content: counter(listCounter);
    display: inline-block;
    margin-right: 6px;
    margin-left: -19px;
    opacity: 0.85;
    text-align: right;
    width: 25px;
    min-width: 25px;
    font-size: 70%;
    color: color-mix(in srgb,rgb(var(--color-blue)) var(--list-items-mix), white);
}
