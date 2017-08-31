# <a name="overview-of-microsoft-graph"></a><span data-ttu-id="93c34-101">Microsoft Graph の概要</span><span class="sxs-lookup"><span data-stu-id="93c34-101">Overview of Microsoft Graph</span></span>

<span data-ttu-id="93c34-p101">Microsoft Graph API を使用すると、Microsoft クラウド内にいるユーザーの、数百万のデータと対話できます。Microsoft Graph を使用して、豊富なリソース、リレーションシップ、インテリジェンスに接続する、組織やコンシューマー向けのアプリケーションを、すべて 1 つのエンドポイントを介して構築します: `https://graph.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="93c34-p101">You can use the Microsoft Graph API to interact with the data of millions of users in the Microsoft cloud. Use Microsoft Graph to build apps for organizations and consumers that connect to a wealth of resources, relationships, and intelligence, all through a single endpoint: `https://graph.microsoft.com`.</span></span>

## <a name="whats-in-the-graph"></a><span data-ttu-id="93c34-104">Graph の内容</span><span class="sxs-lookup"><span data-stu-id="93c34-104">What's in the graph?</span></span>

<span data-ttu-id="93c34-p102">Microsoft Graph は、リレーションシップによって接続されたリソースで構成されています。たとえば、ユーザーは [memberOf](../api-reference/v1.0/api/user_list_memberof.md) リレーションシップを介してグループに、[manager](../api-reference/v1.0/api/user_list_manager.md) リレーションシップを介して別のユーザーに接続できます。アプリはこれらのリレーションシップをスキャンして、これらの接続されたリソースにアクセスし、API を介してそれらのアクションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="93c34-p102">Microsoft Graph is made up of resources connected by relationships. For example, a user can be connected to a group through a [memberOf](../api-reference/v1.0/api/user_list_memberof.md) relationship, and to another user through a [manager](../api-reference/v1.0/api/user_list_manager.md) relationship. Your app can traverse these relationships to access these connected resources and perform actions on them through the API.</span></span>

<span data-ttu-id="93c34-p103">また、Microsoft Graph のデータに関する貴重な洞察とインテリジェンスを得ることもできます。たとえば、特定のユーザーで人気のあるファイルを[トレンド](../api-reference/beta/resources/insights_trending.md)にしたり、ユーザーに最も関連性の高い[人](../api-reference/beta/api/user_list_people.md)を取得したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="93c34-p103">You can also get valuable insights and intelligence about the data from Microsoft Graph. For example, you can get the popular files [trending around](../api-reference/beta/resources/insights_trending.md) a particular user, or get the most relevant [people](../api-reference/beta/api/user_list_people.md) around a user.</span></span>

<span data-ttu-id="93c34-110">Microsoft Graph のリレーションシップが持つ可能性を見つけてください。</span><span class="sxs-lookup"><span data-stu-id="93c34-110">Discover the possibilities in the relationships within Microsoft Graph.</span></span>

![Graph の一部である主要なリソースとリレーションシップを示すイメージ](images/microsoft_graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a><span data-ttu-id="93c34-112">Microsoft Graph でできること</span><span class="sxs-lookup"><span data-stu-id="93c34-112">What can you do with Microsoft Graph?</span></span> 

<span data-ttu-id="93c34-p104">Microsoft Graph を使用すると、ユーザーの固有のコンテキストに関するエクスペリエンスを構築し、生産性を高めることができます。次のアプリを想像してみてください。</span><span class="sxs-lookup"><span data-stu-id="93c34-p104">You can use Microsoft Graph to build experiences around the user's unique context to help them be more productive. Imagine an app that...</span></span>

- <span data-ttu-id="93c34-115">出席者にプロファイル情報を提供することで、次の会議の調査や準備に役立ちます。情報には、出席者の役職や仕事仲間、作業中の最新のドキュメントやプロジェクトに関する情報などが含まれます。</span><span class="sxs-lookup"><span data-stu-id="93c34-115">Looks at your next meeting and helps you prepare for it by providing profile information for attendees, including their job titles and who they work with, as well as information on the latest documents and projects they're working on.</span></span>
- <span data-ttu-id="93c34-116">予定表をスキャンして、次のチームミーティングに最適な時間を提案します。</span><span class="sxs-lookup"><span data-stu-id="93c34-116">Scans your calendar, and suggests the best times for the next team meeting.</span></span>
- <span data-ttu-id="93c34-117">OneDrive の Excel ファイルから最新の売上予測チャートを取得し、リアルタイムで予測を更新します。これらをすべて携帯電話から行います。</span><span class="sxs-lookup"><span data-stu-id="93c34-117">Fetches the latest sales projection chart from an Excel file in your OneDrive and lets you update the forecast in real time, all from your phone.</span></span>
- <span data-ttu-id="93c34-118">予定表の変更を購読したり、会議に時間がかかりすぎているときに警告を送信したり、出席者との関連度に基づいて、見逃しや委任が可能な推奨事項を提示したりします。</span><span class="sxs-lookup"><span data-stu-id="93c34-118">Subscribes to changes in your calendar, sends you an alert when you’re spending too much time in meetings, and provides recommendations for the ones you could miss or delegate based on how relevant the attendees are to you.</span></span>
- <span data-ttu-id="93c34-119">たとえば、個人の OneDrive に送信する必要のある写真と OneDrive for Business に送信する必要のあるビジネスの領収書を分類するなどにより、携帯電話で個人情報や仕事情報を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="93c34-119">Helps you sort out personal and work information on your phone; for example, by categorizing pictures that should go to your personal OneDrive and business receipts that should go to your OneDrive for Business.</span></span>

<span data-ttu-id="93c34-120">Microsoft Graph API を使用すると、これ以上のことができます。</span><span class="sxs-lookup"><span data-stu-id="93c34-120">You can do all this and more with the Microsoft Graph API.</span></span>

## <a name="next-steps"></a><span data-ttu-id="93c34-121">次の手順</span><span class="sxs-lookup"><span data-stu-id="93c34-121">Next steps</span></span>

- <span data-ttu-id="93c34-122">[おすすめのシナリオ](../concepts/featured_scenarios.md)を確認します。</span><span class="sxs-lookup"><span data-stu-id="93c34-122">Check out some [Featured scenarios](../concepts/featured_scenarios.md).</span></span>
- <span data-ttu-id="93c34-123">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)でサンプルの要求を試します。</span><span class="sxs-lookup"><span data-stu-id="93c34-123">Try a sample request in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer)</span></span>
- <span data-ttu-id="93c34-124">[クイック スタート](https://developer.microsoft.com/graph/quick-start)を使用して、すぐに実行できるサンプル アプリをセットアップします。</span><span class="sxs-lookup"><span data-stu-id="93c34-124">Use the [quick start](https://developer.microsoft.com/graph/quick-start) to set up a ready-to-run sample app.</span></span>
- <span data-ttu-id="93c34-125">アプリで[認証トークンを取得する](../concepts/auth_overview.md)方法を検索します。</span><span class="sxs-lookup"><span data-stu-id="93c34-125">Find out how to [get an auth token](../concepts/auth_overview.md) in your app.</span></span>
- <span data-ttu-id="93c34-126">[API の使用](../concepts/use_the_api.md)を開始します。</span><span class="sxs-lookup"><span data-stu-id="93c34-126">Start [using the API](../concepts/use_the_api.md).</span></span>

## <a name="feedback"></a><span data-ttu-id="93c34-127">フィードバック</span><span class="sxs-lookup"><span data-stu-id="93c34-127">Feedback?</span></span>

<span data-ttu-id="93c34-p105">お客様からのフィードバックを重視しています。[スタック オーバーフロー](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph)でご連絡いただけます。ご質問には {MicrosoftGraph} のタグを付けてください。</span><span class="sxs-lookup"><span data-stu-id="93c34-p105">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph). Tag your questions with {MicrosoftGraph}.</span></span>

