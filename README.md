```
        .///.                .///.     //.            .//  `/////////////-
       `++:++`              .++:++`    :++`          `++:  `++:......---.`
      `/+: -+/`            `++- :+/`    /+/         `/+/   `++.
      /+/   :+/            /+:   /+/    `/+/        /+/`   `++.
  -::/++::`  /+:       -::/++::` `/+:    `++:      :++`    `++/:::::::::.
  -:+++::-`  `/+:      --++/---`  `++-    .++-    -++.     `++/:::::::::.
   -++.       .++-      -++`       .++.    .++.  .++-      `++.
  .++-         -++.    .++.         -++.    -++``++-       `++.
 `++:           :++`  .++-           :++`    :+//+:        `++:----------`
 -/:             :/-  -/:             :/.     ://:         `/////////////-
```

# Aave protocol interface :ghost:

An open source interface for the decentralized liquidity protocol Aave

Enabling users to:

- Manage and monitor their positions on the Aave Protocol, and the overall status of it
- Manage and monitor their positions on the Aave Safety module
- Participate on the Aave Governance

## IPFS deployment

Each commit gets deployed to IPFS automatically

There's a github action commenting the appropriate IPFS hash embedded in the Cloudflare IPFS gateway after each commit

For ease of use:

- the DNS of [https://staging.aave.com](https://staging.aave.com) will always point to the latest master IPFS hash with all networks enabled
- the DNS of [https://app.aave.com](https://app.aave.com) will always point to the latest master IPFS hash with disabled test networks

## Troubleshooting

Issue: I cannot connect to `app.aave.com`

The aave-ui is hosted on IPFS in a decentralized manner. `app.aave.com` just holds a CNAME record to the Cloudflare IPFS gateway. You can use [any](https://ipfs.github.io/public-gateway-checker/) public or private IPFS gateway supporting origin isolation to access aave-ui if for some reason the Cloudflare gateway doesn't work for you

Just go to `<your favorite public ipfs gateway>/ipns/app.aave.com`

⚠️ Make sure the gateway supports origin isolation to avoid possible security issues: you should be redirected to URL that looks like `https://app-aave-com.<your gateway>`

### Links known to work at some point:

- [https://app-aave-com.ipns.cf-ipfs.com/#/](https://app-aave-com.ipns.cf-ipfs.com/#/)
- [https://app-aave-com.ipns.dweb.link/#/](https://app-aave-com.ipns.dweb.link/#/)

## Contribution

For instructions on local development, deployment and configurations, see [Contributing](./CONTRIBUTING.md)

## Verification

For instructions on verifying the contract addresses you are interacting with, see [Verification](./VERIFICATION.md)

## License

[BSD-3-Clause](./LICENSE.md)

## Credits

To all the Ethereum community
