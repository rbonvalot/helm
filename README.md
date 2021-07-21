On master

Purge .deploy
<pre>rm -f .deploy/*</pre>
Update your charts
Upload it

<pre>cr upload -o rbonvalot -r helm -p .deploy --token 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</pre>

On gh-pages (orphaned branch)
<pre>cr index -i index.yaml -o rbonvalot -r helm -p .deploy --token ghp_q0Cs7VSbI116krhVPedvtHh
Hf8oQc22qyyLb</pre>
