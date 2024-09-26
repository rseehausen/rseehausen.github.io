layout: page
title: "WHATCOM-CLEANER"
permalink: /whatcomcleaner

<script>
  // Initialize the agent on page load.
  const fpPromise = import('https://fpjscdn.net/v3/ayF4rBJReDGzpx5ktqGP')
    .then(FingerprintJS => FingerprintJS.load())

  // Get the visitorId when you need it.
  fpPromise
    .then(fp => fp.get())
    .then(result => {
      const visitorId = result.visitorId
      console.log(visitorId)
    })
</script>
