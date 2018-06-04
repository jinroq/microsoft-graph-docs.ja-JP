# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="ecc2a-101">SharePoint のサイトおよびコンテンツ API の概要</span><span class="sxs-lookup"><span data-stu-id="ecc2a-101">SharePoint sites and content API overview</span></span>

<span data-ttu-id="ecc2a-102">SharePoint は、インテリジェントなモバイル イントラネットです。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-102">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="ecc2a-103">SharePoint によりユーザーは、コンテンツ、知識、アプリケーションを共有および管理して、チームワークを推進したり、情報を検索したり、組織を通じて共同作業をしたりできます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-103">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="ecc2a-104">Microsoft Graph で SharePoint REST API を使用することにより、ソリューションを SharePoint のサイトおよびコンテンツに統合することができます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-104">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="ecc2a-105">SharePoint のサイトおよびコンテンツを統合する理由</span><span class="sxs-lookup"><span data-stu-id="ecc2a-105">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="ecc2a-106">SharePoint のサイトは、チームのコラボレーションとコミュニケーションを強化します。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-106">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="ecc2a-107">Office 365 のグループ、Microsoft Teams、およびポータルは、すべて SharePoint に基づいているため、Microsoft Graph を使用することにより、保存場所に関係なくデータにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-107">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="ecc2a-108">Microsoft Graph で SharePoint API を使用することにより、次のものにアクセスできます:</span><span class="sxs-lookup"><span data-stu-id="ecc2a-108">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="ecc2a-109">ユーザーが同僚と共同作業するコンテンツを保存するチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-109">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="ecc2a-110">ユーザーが、情報豊富なコンテンツ ページを組織内で共有するために公開する場所となるコミュニケーション サイトおよびポータル。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-110">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="ecc2a-111">SharePoint のリストによりデータを最大限活用する</span><span class="sxs-lookup"><span data-stu-id="ecc2a-111">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="ecc2a-112">[リスト][リスト]は、SharePoint におけるデータ ストレージの基盤となるものです。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-112">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="ecc2a-113">[リストを作成][作成]して、シンプルな顧客連絡先リストからカスタム ビジネス アプリケーションに至るまで、さまざまなビジネス データを保存します。フロントエンドとして PowerApps が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-113">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="ecc2a-114">[列][]を使用してスキーマを定義すると、SharePoint により、そのデータの整合性が保護され、インデックス作成、クエリ、検索の豊富な機能が提供されます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-114">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="ecc2a-115">チームのファイルにリストの強力な機能を提供</span><span class="sxs-lookup"><span data-stu-id="ecc2a-115">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="ecc2a-116">SharePoint は、ドキュメント ライブラリと呼ばれる特殊な[リスト タイプ][]にファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-116">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="ecc2a-117">[OneDrive API][] を使用することにより 1 つの[ドライブ][]としてライブラリを操作したり、SharePoint API を使用することにより[リスト][]として操作したりできます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-117">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="ecc2a-118">通常のリストと同じように、ドキュメント ライブラリのスキーマを拡張して、カスタム列によりビジネス ニーズをサポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-118">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="ecc2a-119">ユーザーの SharePoint イントラネット データによりアプリをライトアップ</span><span class="sxs-lookup"><span data-stu-id="ecc2a-119">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="ecc2a-120">Microsoft Graph により、ユーザーにとって最も重要なデータをアプリ内の前面に打ち出すことができます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-120">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="ecc2a-121">ユーザーのデータを保存したリストに対する[クエリ][]により、常に最新の状態を保ちます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-121">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="ecc2a-122">アプリのための独自のリストを[作成][]し、ユーザーが他の SharePoint エクスペリエンスでそのデータにアクセスするようにしたり、あるいは一切を非表示にしたりします。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-122">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="ecc2a-123">Microsoft Graph を使用して SharePoint を拡張する</span><span class="sxs-lookup"><span data-stu-id="ecc2a-123">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="ecc2a-124">プラットフォームとして SharePoint は、拡張や統合のためのいくつかのモデルを提供します:</span><span class="sxs-lookup"><span data-stu-id="ecc2a-124">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="ecc2a-125">[SharePoint Framework][] は、SharePoint ページでホスト可能なクライアント サイドのテクノロジおよびオープン ソース ツールを使用して Web パーツを作成する手段を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-125">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="ecc2a-126">[SharePoint アドイン][]は、カスタム コードをサーバー上で実行することなく SharePoint サイトに追加することのできる自己完結型拡張機能です。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-126">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="ecc2a-127">アプリが SharePoint ページ内で実行される際、Microsoft Graph を使用することにより、Office 365 を通じて容易にデータにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-127">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="ecc2a-128">それらのモデルに関する詳細については、[SharePoint デベロッパー センター][]または [SharePoint 開発者向けドキュメント][]を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-128">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="next-steps"></a><span data-ttu-id="ecc2a-129">次の手順</span><span class="sxs-lookup"><span data-stu-id="ecc2a-129">Next steps</span></span>

<span data-ttu-id="ecc2a-130">Microsoft Graph の SharePoint を利用する手始めとして、[サイトの使用][SharePoint]についてご確認ください。</span><span class="sxs-lookup"><span data-stu-id="ecc2a-130">Get started with SharePoint in Microsoft Graph by learning more about [working with sites][SharePoint].</span></span>

[リスト]: ../api-reference/v1.0/resources/list.md
[list]: ../api-reference/v1.0/resources/list.md
[列]: ../api-reference/v1.0/resources/columndefinition.md
[columns]: ../api-reference/v1.0/resources/columndefinition.md
[リスト タイプ]: ../api-reference/v1.0/resources/listinfo.md
[List Type]: ../api-reference/v1.0/resources/listinfo.md
[作成]: ../api-reference/v1.0/api/list_create.md
[create]: ../api-reference/v1.0/api/list_create.md
[クエリ]: ../api-reference/v1.0/api/listitem_get.md
[querying]: ../api-reference/v1.0/api/listitem_get.md
[ドライブ]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
<span data-ttu-id="ecc2a-137">
  [OneDrive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive</span><span class="sxs-lookup"><span data-stu-id="ecc2a-137">[OneDrive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive</span></span>
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint アドイン]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint デベロッパー センター]: https://developer.microsoft.com/sharepoint
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[SharePoint 開発者向けドキュメント]: http://aka.ms/spdev-docs
[SharePoint Developer Docs]: http://aka.ms/spdev-docs
[SharePoint]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/sharepoint
