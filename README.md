# Repolex Knowledge Graph of pytorch/data

RDF knowledge graph data for [pytorch/data](https://github.com/pytorch/data), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download pytorch/data
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 2965fd3ec0f93241dfcd27a3a23bc14a5fc4ecec
│   │   │   └── chunk-001.nq.gz
│   │   └── ee79a399d3a53676544e0d3f0e826ffa58d1fec9
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 2965fd3ec0f93241dfcd27a3a23bc14a5fc4ecec.nq.gz
│   └── repolex
│       ├── 2965fd3ec0f93241dfcd27a3a23bc14a5fc4ecec
│       │   └── chunk-001.nq.gz
│       └── ee79a399d3a53676544e0d3f0e826ffa58d1fec9
│           └── chunk-001.nq.gz
└── blob
    ├── 00b6db8269468857e03dbfc296f3fcf7c173538b.nq.gz
    ├── 0104076bb3f146a4a7029536930401bc2d00a250.nq.gz
    ├── 043682aafd586056df747c526bd159e9015a022f.nq.gz
    ├── 04a9702f516409f4a075474595504c7c4d855cb4.nq.gz
    ├── 05be60b5155716aef202f0f7dc436a19fc0407e8.nq.gz
    ├── 06136dace59239b47183727b1988d8215ae7ea9b.nq.gz
    ├── 061e802825a69f6aa0283f47591c5ba51ec3dba3.nq.gz
    ├── 061f32f91b96f05f8fa2b52b2edcdcc19aa33d50.nq.gz
    ├── 0683862661bd5cf64cc28b78d9619929a4da872d.nq.gz
    ├── 075ad3ef8bf5aae111251b6894a0d08529713a3c.nq.gz
    ├── 087ba842d2a7e104d58dfb64c2ba70f4ed71ec5b.nq.gz
    ├── 094f41d31b55799355cfa2acdfa1dd98347c0434.nq.gz
    ├── 095e0f4f32be28f922976e2b72af0921980940e4.nq.gz
    ├── 09ab0fa4f105afd53212e33440fc39727a4cb25e.nq.gz
    ├── 0a775552cbe697faf8f065b9e211af27ea5a64a0.nq.gz
    ├── 0a971b0e3e0e1c78dcb0c518de76fe764827c070.nq.gz
    ├── 0c8332c155c86b9490cf15731472fc79443a9e46.nq.gz
    ├── 0d02f738b0d017fed00450e1fe008c8f9d1b1971.nq.gz
    ├── 0d3f45970d4a57e959bbe789fc67b654abc71a61.nq.gz
    ├── 0ed27a48547369e01d5c43ad2605cbd86ac96bde.nq.gz
    ├── 0f3f102dce2a390a2c58dfc3137fd0ac81e44125.nq.gz
    ├── 0fa29eff0d2f6303f3c1ec21f32a4a65d89b08cb.nq.gz
    ├── 10866ec73f6cadf02f293839d40b32b40516912e.nq.gz
    ├── 108f269ece884b34576fa94595f02e2300b59ab4.nq.gz
    ├── 10cdd8964adf3bf4e0f5984356427e57410af199.nq.gz
    ├── 1203e7f75cb0d60ce8266c91e5a4b433a5f05ec1.nq.gz
    ├── 13221e163ab6e9463e7161fac69be8cc48b9bba5.nq.gz
    ├── 136189c7dcfa6207f1078fa38b34a8cc44573337.nq.gz
    ├── 13cdc42e13beeab34819ff88286fec62bb84442c.nq.gz
    ├── 143d976799609fa24f675fab8a91c701714a9440.nq.gz
    ├── 147066f3495514bee649dec9f5880228d35d0f15.nq.gz
    ├── 14a4b8fa8008dda92c422b65643ee20ca7a1d3d6.nq.gz
    ├── 14ca32cdb4d3c23bb3fdd382189df0f56d89ddc3.nq.gz
    ├── 152081576186113a384189212d329ab498af14ae.nq.gz
    ├── 162246b881a763ab75d7b49c5962a00d9663128d.nq.gz
    ├── 16638d1d020d989f9e26f60e5570b35979b4b20f.nq.gz
    ├── 181a91f74f382fe04f3c3685f21f3db4878519d7.nq.gz
    ├── 1af26f875e976644725d0098afe4e5ca76df5cae.nq.gz
    ├── 1bd3dbced7ed7335dfb95cac840fb6b4db313d55.nq.gz
    ├── 1db0155da240ebe289015c85b593ad616321a9cc.nq.gz
    ├── 1e84df4e5cca306eb1e72461adbdba39e331803c.nq.gz
    ├── 1ed20b5fa395de92505e388067128e2c12c0ec6a.nq.gz
    ├── 1f014acb92200abe62a5e4d2eb5baeeec9ba83b0.nq.gz
    ├── 1f5e7c9ef90bf510a5de4e819fe472034bee2d25.nq.gz
    ├── 241ae046f5e0d6bb7e9edcdd666de974a1f3402e.nq.gz
    ├── 2472356824570ee169b7a86f6539127c57f7025c.nq.gz
    ├── 25bb523ac833d713ebdd6f5672f340d154e673d3.nq.gz
    ├── 25dd69c703a59e05f3d2dba25a807dc833d3eace.nq.gz
    ├── 26416e8bcd10d5f9862b04dacc6842015f04d0fe.nq.gz
    ├── 2661eec9c0cb6f3d7dc8170bf2ea0f996f15de00.nq.gz
    ├── 28ef872d8b8d7b1a51249973ddcd68bbf89ca50c.nq.gz
    ├── 2905325bdd7684583ee0e0308a3fcba64d79c882.nq.gz
    ├── 2972122f9dd7b69174a82d61c3b9c76cf2e4950d.nq.gz
    ├── 29da914fd8395702e88d242122715344a008e5e8.nq.gz
    ├── 29f64b083715ac5d68ed6877f4078bdff951e8d8.nq.gz
    ├── 2a358b6a3c7e020db856bdc179316243edc0ff8d.nq.gz
    ├── 2a5a50ab287faf4808a9ba2d736a0a2db357330a.nq.gz
    ├── 2a74a5642dd22002799d3cc1161ab0b2b00a18e6.nq.gz
    ├── 2b6e328b98366306f1db93e369379f6595357751.nq.gz
    ├── 2b9895351e598f1a6ca0250f5f98adad8cf3966f.nq.gz
    ├── 2bac575bfbaf22aab29e12d1043aa82b61990f46.nq.gz
    ├── 2c95d0e0a54fe70559ea694f58d41e8b9d3a4d67.nq.gz
    ├── 2de235eb30dd0544b6b71389073029b54381721e.nq.gz
    ├── 2e41cd717f6a439a9c08d76a9d0e4a54e190fc5a.nq.gz
    ├── 2f6442ac9bd048dac53567b98bc3f41de05a0f22.nq.gz
    ├── 2fb369acfde7f3b17e90e54fda494e5ec9f44c44.nq.gz
    ├── 309f2312c3eb9d3fc9ed3146523fcfdbb49de1a7.nq.gz
    ├── 30f42b317d97167bdbc6599b8668721a621946b5.nq.gz
    ├── 313b5e361785b17aafb37d8af91ca6a86a8c229c.nq.gz
    ├── 32676c78c6ed672aa2a801a52a31ee25f4b0f5ae.nq.gz
    ├── 3348e0a99d70a0e3134bdbc7a7c6d470b641e2fd.nq.gz
    ├── 3391a3dcca1976d957775d568456bd14648bae8f.nq.gz
    ├── 33aff5e6eefe4c50dfec7703d975f248106c2288.nq.gz
    ├── 33c05350541bd3259655ac035a1030c37b6e490e.nq.gz
    ├── 37365a81ce0a10d1a03cc520d6c9ac6f8130e5c5.nq.gz
    ├── 39a875a94a3167546bbe1d3260659648c5df8782.nq.gz
    ├── 3a8f4b9823ef202ce030650bb31e1fae41e4a451.nq.gz
    ├── 3b6d08ea2392dc8e48c76c385d1ff501b16e812c.nq.gz
    ├── 3b77c094a004801f4965cf7a67a8387fd8baed79.nq.gz
    ├── 3c2dd4df8af84e1224ad757e2c681d3586cd6485.nq.gz
    ├── 3c76d910ca604f923b2eb1ea17408be2983fdbbc.nq.gz
    ├── 3ce401c273f3fba273a70f345641c6dc38738a44.nq.gz
    ├── 3d82fc151855e99dabf20fdc31864892486da349.nq.gz
    ├── 3db2940af4882aa734e01ea2a8a87f95851ffbd5.nq.gz
    ├── 3dd248408b46732d0e2aecb21d649a2ca79f1642.nq.gz
    ├── 3deb3f53ba40bdb5267cd0dc5131c5b38b342153.nq.gz
    ├── 3e64869d69c276fdb6e91e03bf41575561d86556.nq.gz
    ├── 3e80eaea21de3a2312910254ba06978537ff8a27.nq.gz
    ├── 3f52f9d9ebdecd03c739ff00fa9102987cb0faf7.nq.gz
    ├── 3f55c1acc8b6f2ffaca72d9b0269d0e0a6c2ea47.nq.gz
    ├── 3f9dd7cf18da1b101a67d198890a810f363d68c9.nq.gz
    ├── 3fb5aea278223639f78470d99fd6195a314e0c85.nq.gz
    ├── 3fc310875544358968bdfea31fd79671e3abec85.nq.gz
    ├── 42642630479834b5940585ccd2687b3bfcf7b07c.nq.gz
    ├── 4317a9479de35665c460df756f50e848017f17de.nq.gz
    ├── 436d3d5d00d515ab61239f5add24014d767350fd.nq.gz
    ├── 438122b9ef79155c94ece771f8fa979839b361c9.nq.gz
    ├── 45bc4c8e31d3b757e97f3f23e6b2202eba4201b2.nq.gz
    ├── 4615761c4a3a7b5bb59a381c1f86904477d1baed.nq.gz
    ├── 4791f933383e74ebeaa2b39fc3a0f13d48a6a88f.nq.gz
    ├── 47cb88dd57ea70b728f05f5edc15a39974dcf2cc.nq.gz
    ├── 4828bd9ed19fdf9ab80f78c70ade0e1a29e85809.nq.gz
    ├── 48780ad8fd4c442c81b90f24a3f329290cf33b4f.nq.gz
    ├── 48f5e0a090ae88a3bb4603e81af6c093b3171868.nq.gz
    ├── 49b37a8a502ce5c4dfc7e9d04a3d13d0e15554c8.nq.gz
    ├── 4a3cf65a4517aa05d7a20185763e2491ad52e01a.nq.gz
    ├── 4a7122b584e6f20098e72031e367643a92763115.nq.gz
    ├── 4ae37eac9da9140e4ecd648a3ffdafd9513692b4.nq.gz
    ├── 4b6c398cb6cd83eb1398a73b37954c9ac85ac800.nq.gz
    ├── 4c46f013cd03652f29c8f74b1f1b1b0b0f441316.nq.gz
    ├── 500d0ba2a960073281554a6cdb2779b875d6e06d.nq.gz
    ├── 53f5bc13ec336c8eef7c7c4368017b7c262ea31f.nq.gz
    ├── 543eb5f464ec6bf3c8234cb8f0323a0ecf6c3956.nq.gz
    ├── 547920d65de9d1b636f1564496b8dcbd5cefd076.nq.gz
    ├── 554b4d8d66a01834aaa13b012ee71cc7303a4c5c.nq.gz
    ├── 55c18a0fdf61ba7c914c672d47e7c8b87d1288a9.nq.gz
    ├── 572534e47fefa478f364672a807c3b185520232b.nq.gz
    ├── 5764a3d6033d6179e8023f28c3291ea97f15dd48.nq.gz
    ├── 57a505b6f75cd1264292b7d77ba2c535b360a17a.nq.gz
    ├── 5859472bf128bc64456b7a7bd9ff9b46a76fd95c.nq.gz
    ├── 58b3cbf9ab9060313c4b62b8627a8a59d38f4ba7.nq.gz
    ├── 5aa5895af9960535ed232b5c8b4b6d5d38fbea81.nq.gz
    ├── 5b7f465516787996ba969b24737fb3a04e8aae12.nq.gz
    ├── 5bec089ef5de6fe8771208912ba34b055234b2d8.nq.gz
    ├── 5fd020924728e61eae2a0d5148040da3f906ed90.nq.gz
    ├── 60219cb940ce615cb4c62ea2290b1d7301e2a18b.nq.gz
    ├── 63d3f393c5ded4d59f9548eb4358ea490a96b3d0.nq.gz
    ├── 64b51dd92d33504df7aaf402bafcc2d013459b04.nq.gz
    ├── 65ed1522b0db20cf8c9479bdb1c30593fe35cd74.nq.gz
    ├── 66a51fa7b77745229717ff4250f3ac7cc3ac89f4.nq.gz
    ├── 66b4f669233caa69ce422853446acca350dd9b3f.nq.gz
    ├── 66c557729adcd9aa59ba4af278727cfb10347174.nq.gz
    ├── 67ccceab60e7961a34692dd192a4967e979ed7bb.nq.gz
    ├── 6832002728981b7906afaed7a2d65ed62160b391.nq.gz
    ├── 68a45259a448fc7bbb2ce8773a4ed6db7392c1ec.nq.gz
    ├── 6ac03dc6a012cc942cb709d4aba70035fc4ccad9.nq.gz
    ├── 6b4f70a85ee351bcc834c0a62040988089e8cc11.nq.gz
    ├── 6ba875f5642a3f8df3ce83ae52e4152d607c0377.nq.gz
    ├── 6d174a24561a38f7a72a06cbde6e2332e869e1cd.nq.gz
    ├── 6e292ad8009c4aa7f4d725727b41b307351af8c5.nq.gz
    ├── 6eea9bd30e35a2c96b6d0fa3f92c6d448dbe10f7.nq.gz
    ├── 7182573a3992616ff0b19728680b497b0bebf724.nq.gz
    ├── 724612e906ef2a1c10ec97ad4853e9e66d782bcf.nq.gz
    ├── 73a54d1c9d370032f1f692f871632c1a5e7a0431.nq.gz
    ├── 73f597e7503da839b67bcf8e9f89274c97a30943.nq.gz
    ├── 754e95b8b1296d5764622b904e84994e9364408a.nq.gz
    ├── 773ba85b15475432ddcad576ebcf14a6436231e9.nq.gz
    ├── 774ec3297800c7cdb5f9f50960c00bc6f25d9a46.nq.gz
    ├── 783f38329fb3c8856348b0d0d4d7afaf272cae8d.nq.gz
    ├── 783fa9fb69c57917b73c232c4b37721bd74f0d2d.nq.gz
    ├── 786ab0b3cd187471f8382c748c0bb362a42aebf1.nq.gz
    ├── 79308ea4c33ea115f3f167400fe5b7160f5900b9.nq.gz
    ├── 7a965dd02a20627b2f3aae896337d72604f9214f.nq.gz
    ├── 7b9d8d9dc98ddddc1b971509e59b589749db2db8.nq.gz
    ├── 7bfc7f93051ebbe00fcbf68ecda67341405537da.nq.gz
    ├── 7c0ac88360196d751de19594a6541b3b64ccf265.nq.gz
    ├── 7d424791ea7bee321cdc4edea3987c10874c8dd1.nq.gz
    ├── 7de04873a944d2d4fba4bc26594d3e7a7abacbd7.nq.gz
    ├── 7e63ce126d11ffc5adbd27b4290bbf30a8bba60b.nq.gz
    ├── 7f4de23510a394ce6c2da12ac2e1cbe8d13845b7.nq.gz
    ├── 800ed8d279f3c4a5ddda75307252eee34fb0539b.nq.gz
    ├── 808b5effada247e265969fce215dac70f16fc69d.nq.gz
    ├── 82214920ff2d63c1a8bb14139052104fb00553b5.nq.gz
    ├── 82c197b8ae3a574810b21d081a72200f3551ebd9.nq.gz
    ├── 851872b3c1e5418f494ce8b33eaf1a1582f99d46.nq.gz
    ├── 86236c7b4b9ae1003d4832e97857991f34f1ef74.nq.gz
    ├── 86a818974801c3b38ffa8a45b5594f434b912082.nq.gz
    ├── 86b9ee38723ffbe3f9978c8e810ac1840eb317c2.nq.gz
    ├── 873046af7ffeb135f368d3fe2a57c013a9aaab4d.nq.gz
    ├── 874b06f4e6ecd878c3878fb07ffe63c8ffe3342f.nq.gz
    ├── 8a0ce2ed244a5d176263931f6f566ee9ce335ef7.nq.gz
    ├── 8a3c1fc82736a7ee9c357dd9d2e5606efc90100a.nq.gz
    ├── 8ad5ea10150e08626081dd87c0f7a38e23513766.nq.gz
    ├── 8cf9d86bf7d5f5cd656c0890abc94e934775eea2.nq.gz
    ├── 8d53ffec07b16d10965e62ed6786a7c29ac671fa.nq.gz
    ├── 8f426115e948f456ec7ab56281905f01be2a68a9.nq.gz
    ├── 8f7cb280024cf81998a66e4c7492fb5a37e3343a.nq.gz
    ├── 900880f1247ebebe07ac69cc5845c11229c42140.nq.gz
    ├── 9079886506d8c46fb2924b046ff78bada60d8f12.nq.gz
    ├── 90f06d964df676f28d761afa4d2c57dbd715f458.nq.gz
    ├── 92a478ad833b9ed9389fa8ed01c0b087f2755f59.nq.gz
    ├── 92ef577afff2a7b8841f10beee486e34d8044e3d.nq.gz
    ├── 931bef182a05326cb23ad06d6767e803af067e91.nq.gz
    ├── 932df2a431b39b513789c9bf01b6c14e458d4f24.nq.gz
    ├── 93cedfd0074e6364511e780ba64b311e81424317.nq.gz
    ├── 93d042ee798e0bb8ff87a97f01fdf9817b69b271.nq.gz
    ├── 943bfbf1236222d2b768fcbf72f2697ccfcc6b02.nq.gz
    ├── 945258b8e870f2aab41f8cee3575e66f85bed7f5.nq.gz
    ├── 9480ecda6ab802aca2d3b4871cec8cc75992a41b.nq.gz
    ├── 94d4b08ab09e51b4c0c73d18663a9ae8d04fa653.nq.gz
    ├── 9523bb703f18cefc0e05e0a5c06a78f57786a358.nq.gz
    ├── 95d97a73abe7fd794cef454120168faeeaf806f6.nq.gz
    ├── 95f3dc319cfe2802db87fff11abf14c6b33c24e9.nq.gz
    ├── 965fbb73dc7045e5116e4456f7dcc52a107557c9.nq.gz
    └── 972c61ff4477769bb77cc0b78f7c26243ee55605.nq.gz

10 directories, 200 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[pytorch/data](https://github.com/pytorch/data)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
