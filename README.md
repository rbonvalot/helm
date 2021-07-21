On master

Purge .deploy
<pre>rm -f .deploy/*</pre>
Create the chart's package
<pre>helm package charts/gitlab-monolith --destination .deploy</pre>
Update your charts
Upload it

<pre>cr upload -o rbonvalot -r helm -p .deploy --token <token></pre>

On gh-pages (orphaned branch)
<pre>cr index -i index.yaml -o rbonvalot -r helm -p .deploy --token <token></pre>


source: https://tech.paulcz.net/blog/creating-a-helm-chart-monorepo-part-1/
