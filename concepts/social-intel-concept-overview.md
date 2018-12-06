---
title: Microsoft Graph におけるソーシャル インテリジェンスと分析の概要
description: Microsoft Graph では、Microsoft 365 のクラウド サービスを使用する何千万人ものユーザーが中核的な役割を果たします。 ユーザーのデータは、慎重に管理、保護されており、適切な権限があれば、Microsoft Graph サービスでビジネスの生産性や創造性を促進するために利用できます。 ユーザーのデータは Microsoft Graph のあらゆる部分に存在しますが、ユーザーの社会的な交流から得られたデータは特に興味深いものがあります。 たとえば、次のような質問への答えを導く知的なインサイトを得ることができます。
ms.openlocfilehash: 518d7cb773ae32199c38f2eb8459d785b2750f18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092480"
---
# <a name="overview-of-social-intelligence-and-analytics-in-microsoft-graph"></a><span data-ttu-id="56473-106">Microsoft Graph におけるソーシャル インテリジェンスと分析の概要</span><span class="sxs-lookup"><span data-stu-id="56473-106">Overview of social intelligence and analytics in Microsoft Graph</span></span>

<span data-ttu-id="56473-107">Microsoft Graph では、Microsoft 365 のクラウド サービスを使用する何千万人ものユーザーが中核的な役割を果たします。</span><span class="sxs-lookup"><span data-stu-id="56473-107">The hundreds of millions of users of Microsoft 365 cloud services form part of the core of Microsoft Graph.</span></span> <span data-ttu-id="56473-108">ユーザーのデータは、慎重に管理、保護されており、適切な権限があれば、Microsoft Graph サービスでビジネスの生産性や創造性を促進するために利用できます。</span><span class="sxs-lookup"><span data-stu-id="56473-108">The users' data is carefully managed, protected, and with proper authorization, made available by Microsoft Graph services to drive productivity and creativity in businesses.</span></span> <span data-ttu-id="56473-109">ユーザーのデータは Microsoft Graph のあらゆる部分に存在しますが、ユーザーの社会的な交流から得られたデータは特に興味深いものがあります。</span><span class="sxs-lookup"><span data-stu-id="56473-109">As ubiquitous the user's data is in Microsoft Graph, data derived from the user's social interactions is particularly interesting.</span></span> <span data-ttu-id="56473-110">たとえば、次のような質問への答えを導く知的なインサイトを得ることができます。</span><span class="sxs-lookup"><span data-stu-id="56473-110">It provides intelligent insights that can answer questions such as the following:</span></span>

- <span data-ttu-id="56473-111">「このユーザーはこのトピックの情報を誰に問い合わせればよいか?」</span><span class="sxs-lookup"><span data-stu-id="56473-111">"Who should this user contact for information on this topic?"</span></span>
- <span data-ttu-id="56473-112">「このユーザーにとって最も関心があるドキュメントはどれか?」</span><span class="sxs-lookup"><span data-stu-id="56473-112">"Which documents are most interesting to this person?"</span></span>

<span data-ttu-id="56473-113">Microsoft Graph では、People API と Insights API を使用してユーザーに関連する人物とドキュメントにアクセスできる、よりスマートなアプリを構築できます。</span><span class="sxs-lookup"><span data-stu-id="56473-113">You can use the people API and insights API in Microsoft Graph to build smarter apps that can, respectively, access the relevant people and documents for a user.</span></span>

<span data-ttu-id="56473-114">People API は、人物をユーザーとの関連性が高い順に返します。これらの人物は、そのユーザーの連絡先、ソーシャル ネットワーク、組織の人名簿、およびメールや Skype で行われた最近のコミュニケーションに基づいて収集されます。</span><span class="sxs-lookup"><span data-stu-id="56473-114">The people API returns people ordered by relevance to a user, based on that user's contacts, social networks, organization directory, and recent communications on email and Skype.</span></span> <span data-ttu-id="56473-115">これは、人物を選択するシナリオで特に有用です。</span><span class="sxs-lookup"><span data-stu-id="56473-115">This is particularly useful for people-picking scenarios.</span></span>

<span data-ttu-id="56473-116">Insights API は、高度な分析と機械学習を使用して、ユーザーが 1 日の作業時間を通して必要とする最も関連性の高いファイルを提供します。</span><span class="sxs-lookup"><span data-stu-id="56473-116">The insights API uses advanced analytics and machine learning to provide the most relevant files users need throughout their work day.</span></span> <span data-ttu-id="56473-117">この API により、Office Delve、SharePoint ホーム、OneDrive for Business の [Discover] ビュー、Outlook on the web などの使い慣れた Office 365 のエクスペリエンスが強化されます。</span><span class="sxs-lookup"><span data-stu-id="56473-117">The API powers familiar Office 365 experiences, including Office Delve, SharePoint Home, the Discover view in OneDrive for Business, and Outlook on the web.</span></span>

![People API と Insights API は、あるユーザーに関連する人物とドキュメントを返します](images/social-intel-concept-overview-data.png)

## <a name="why-integrate-with-people-data"></a><span data-ttu-id="56473-119">人物のデータと統合する理由</span><span class="sxs-lookup"><span data-stu-id="56473-119">Why integrate with people data?</span></span>

<span data-ttu-id="56473-120">People API は、1 つのエンティティ ([person](/graph/api/resources/person?view=graph-rest-1.0)) のデータを返します。このエンティティには、今日のビジネスの世界における個人の一般的なデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="56473-120">The people API returns data of a single entity, [person](/graph/api/resources/person?view=graph-rest-1.0), which includes typical data of an individual in today's business world.</span></span> <span data-ttu-id="56473-121">Microsoft Graph ユーザーにとって、この **person** データを特に便利なものにしているのが、その_関連性_です。</span><span class="sxs-lookup"><span data-stu-id="56473-121">What makes this **person** data especially useful is its _relevance_ with respect to a Microsoft Graph user.</span></span> <span data-ttu-id="56473-122">関連性は、ユーザーのコミュニケーションやコラボレーションのパターン、およびビジネス リレーションシップに基づいて計算される各人物の関連性スコアで示されます。</span><span class="sxs-lookup"><span data-stu-id="56473-122">Relevance is noted in a relevance score of each person, calculated based on the user's communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="56473-123">この_関連性_データの用途には 3 つのタイプがあります。</span><span class="sxs-lookup"><span data-stu-id="56473-123">There are 3 main types of application of this _relevance_ data.</span></span>

### <a name="browse-people-by-relevance"></a><span data-ttu-id="56473-124">関連性による人物の参照</span><span class="sxs-lookup"><span data-stu-id="56473-124">Browse people by relevance</span></span>

<span data-ttu-id="56473-125">適切な[権限](people-example.md#authorization)を取得すると、サインインしているユーザー、またはサインインしているユーザーの組織内の他のユーザーに関連する人物を参照できます。</span><span class="sxs-lookup"><span data-stu-id="56473-125">You can browse people who are related to the signed-in user or to some other user in the signed-in user's organization, provided you have got the appropriate [authorization](people-example.md#authorization).</span></span> <span data-ttu-id="56473-126">ユーザーは、関連性の順に並べられた **person** オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="56473-126">You get a collection of **person** objects that are ordered by relevance.</span></span> <span data-ttu-id="56473-127">応答で返された **person** オブジェクトのコレクションは、クエリ パラメーター `top`、`skip`、`orderby`、`select`、および `filter` を指定することでさらに[カスタマイズ](people-example.md#browse-people)できます。</span><span class="sxs-lookup"><span data-stu-id="56473-127">You can further [customize](people-example.md#browse-people) the collection of **person** objects that is returned in the response by specifying the query parameters `top`, `skip`, `orderby`, `select`, and `filter`.</span></span>

### <a name="fuzzy-searches-based-on-people-criteria"></a><span data-ttu-id="56473-128">人物の抽出条件に基づくあいまい検索</span><span class="sxs-lookup"><span data-stu-id="56473-128">Fuzzy searches based on people criteria</span></span>

<span data-ttu-id="56473-129">アプリがサインインしているユーザーによるアクセス許可を取得している場合は、People API でそのユーザーに関連する人物を検索できます </span><span class="sxs-lookup"><span data-stu-id="56473-129">The people API lets you search for people relevant to the signed-in user, provided that your app has got permissions by that user.</span></span> <span data-ttu-id="56473-130">(詳細については、「[People のアクセス許可](permissions-reference.md#people-permissions)」を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="56473-130">(Read more on [people permissions](permissions-reference.md#people-permissions).)</span></span>

<span data-ttu-id="56473-131">あいまい検索により、完全に一致する項目と、検索目的の推論に基づく結果が返されます。</span><span class="sxs-lookup"><span data-stu-id="56473-131">Fuzzy searches return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="56473-132">これを具体的に示す次の例では、サインインしているユーザーに関連し、名前_またはメール アドレス_に「j」で始まる単語が含まれている **person** オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="56473-132">To illustrate this, the following example returns **person** objects relevant to the signed-in user whose name, _or email address_, contains a word that starts with 'j'.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search=j
```

### <a name="fuzzy-searches-based-on-topic-criteria"></a><span data-ttu-id="56473-133">トピックの抽出条件に基づくあいまい検索</span><span class="sxs-lookup"><span data-stu-id="56473-133">Fuzzy searches based on topic criteria</span></span>

<span data-ttu-id="56473-134">People API では、サインインしているユーザーに関連し、そのユーザーと特定の「トピック」についてやり取りしたいと言っている人物を検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="56473-134">The people API also lets you perform searches for people who are relevant to the signed-in user, and have expressed an interest in communicating with that user over certain "topics".</span></span> <span data-ttu-id="56473-135">トピックとは、ユーザーが電子メールの会話で最もよく使用している単語のことです。</span><span class="sxs-lookup"><span data-stu-id="56473-135">Topics are just words that have been used most by users in email conversations.</span></span> <span data-ttu-id="56473-136">Microsoft はそのような単語を抽出し、コンテキストを取り除き、そのデータのインデックスを作成してあいまい検索を容易にします。</span><span class="sxs-lookup"><span data-stu-id="56473-136">Microsoft extracts such words, free of their contexts, and creates an index for this data to facilitate fuzzy searches.</span></span>

<span data-ttu-id="56473-137">次の例は、「カブトムシ」というトピックの検索目的の推論を示しています。</span><span class="sxs-lookup"><span data-stu-id="56473-137">The following example illustrates inferences about the intent of a search on the topic "beetle":</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search="topic:beetle" 
```

<span data-ttu-id="56473-138">トピック データのインデックスのあいまい検索により、昆虫のカブトムシ、フォルクス ワーゲンの象徴的な車であるビートル、バンドのビートルズ、およびその他の定義のインスタンスが返されます。</span><span class="sxs-lookup"><span data-stu-id="56473-138">A fuzzy search in the topic data index return instances that mean the beetle insect, the iconic Volkswagen Beetle car, the Beatles band, and other definitions.</span></span>


## <a name="why-integrate-with-document-based-insights-preview"></a><span data-ttu-id="56473-139">ドキュメントベースのインサイト (プレビュー) と統合する理由</span><span class="sxs-lookup"><span data-stu-id="56473-139">Why integrate with document-based insights (preview)?</span></span>

### <a name="use-intelligence-to-improve-collaboration"></a><span data-ttu-id="56473-140">インテリジェンスを使用したコラボレーションの改善</span><span class="sxs-lookup"><span data-stu-id="56473-140">Use intelligence to improve collaboration</span></span>

<span data-ttu-id="56473-141">ユーザーは多くの場合、通常の 1 日の作業時間中に、多くのドキュメントに保存されている大量の情報を操作し、さまざまな方法で他のユーザーと共同作業を行います。</span><span class="sxs-lookup"><span data-stu-id="56473-141">During a typical work day, users often interact with large amounts of information stored across many documents and collaborate with other users in many different ways.</span></span> <span data-ttu-id="56473-142">必要な情報が必要なときに常に見つかることが重要です。</span><span class="sxs-lookup"><span data-stu-id="56473-142">It's important that they can always can find what they need, when they need it.</span></span>

<span data-ttu-id="56473-143">[trending](/graph/api/resources/insights-trending?view=graph-rest-beta)、[shared](/graph/api/resources/insights-shared?view=graph-rest-beta)、および [used](/graph/api/resources/insights-used?view=graph-rest-beta) API を含む Insights API を使用して、ユーザーの現在のコンテキストとニーズに基づいて Office 365 全体からファイルを抽出することにより、ユーザーの生産性が向上し、組織内のコラボレーションが改善されます。</span><span class="sxs-lookup"><span data-stu-id="56473-143">You can use the insights API, which includes the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta), [shared](/graph/api/resources/insights-shared?view=graph-rest-beta), and [used](/graph/api/resources/insights-used?view=graph-rest-beta) APIs, to surface files from across Office 365 based on your users' current context and needs, making users more productive and improving collaboration in your organization.</span></span>

<span data-ttu-id="56473-144">アプリでは、Insights API の結果を簡単にレンダリングできます。</span><span class="sxs-lookup"><span data-stu-id="56473-144">It is easy to render the results from the insights API in your app.</span></span> <span data-ttu-id="56473-145">すべての結果には、プレビュー イメージの URL やプレビュー テキストなどの一般的な視覚化プロパティのセットが付属しています。</span><span class="sxs-lookup"><span data-stu-id="56473-145">Every result comes with a set of common visualization properties, like a preview image URL or preview text.</span></span>

### <a name="make-relevant-content-visible"></a><span data-ttu-id="56473-146">関連するコンテンツの視覚化</span><span class="sxs-lookup"><span data-stu-id="56473-146">Make relevant content visible</span></span>

<span data-ttu-id="56473-147">Office 365 の Delve では、_trending_ のインサイトを使用して、ユーザーが現在最も興味を持っているドキュメントを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="56473-147">In Office 365, Delve uses the _trending_ insight to help users discover the documents that are most interesting to them right now.</span></span> <span data-ttu-id="56473-148">図 1 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56473-148">See figure 1.</span></span>

<span data-ttu-id="56473-149">プログラムの中で Insights API の [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) エンティティを使用すると、アプリの顧客に同じようなエクスペリエンスを提供できます。</span><span class="sxs-lookup"><span data-stu-id="56473-149">Programmatically, you can use the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) entity in the insights API to provide your app customers a similar experience.</span></span> <span data-ttu-id="56473-150">**trending** エンティティを使用して、ユーザーが最近話題にしているドキュメントやユーザーに関連するドキュメントに接続します。</span><span class="sxs-lookup"><span data-stu-id="56473-150">Use the **trending** entity to connect to documents that are trending around and relevant to the user.</span></span> <span data-ttu-id="56473-151">[人気上昇中のドキュメントの一覧表示](/graph/api/insights-list-trending?view=graph-rest-beta)では、OneDrive または SharePoint のチーム サイトに保存されているファイルが、関連性の最も高いものから順に並べ替えて返されます。</span><span class="sxs-lookup"><span data-stu-id="56473-151">[Listing trending documents](/graph/api/insights-list-trending?view=graph-rest-beta) returns those files stored on OneDrive or SharePoint team sites, sorted by relevance with the most important ones first.</span></span> 

<span data-ttu-id="56473-152">**図 1 あるユーザーに人気のあるドキュメントが表示されている Office 365 の Delve**</span><span class="sxs-lookup"><span data-stu-id="56473-152">**Figure 1. Delve in Office 365 showing popular documents for a user**</span></span>

![あるユーザーに人気のあるドキュメントが表示されている Office 365 の Delve のスクリーンショット](images/delve-concept.png)

### <a name="allow-users-to-collaborate-and-get-back-to-work"></a><span data-ttu-id="56473-154">ユーザーが共同作業の後で作業に戻れるようにする</span><span class="sxs-lookup"><span data-stu-id="56473-154">Allow users to collaborate and get back to work</span></span>

<span data-ttu-id="56473-155">新しい Office 365 の人物カードは、_used_ および _shared_ のインサイトを利用して人物と知識単位を結びます。</span><span class="sxs-lookup"><span data-stu-id="56473-155">The new Office 365 people cards tap into the _used_ and _shared_ insights to connect the dots between people and units of knowledge.</span></span> <span data-ttu-id="56473-156">人物カードは、あるユーザーに関連するドキュメントを識別し、表示します。</span><span class="sxs-lookup"><span data-stu-id="56473-156">The people card identifies and displays relevant documents about a person.</span></span> <span data-ttu-id="56473-157">ユーザーは、Outlook on the web など、スイート全体で人物カードを表示できます。</span><span class="sxs-lookup"><span data-stu-id="56473-157">Users can see people cards across the suite, for example, in Outlook on the web.</span></span> <span data-ttu-id="56473-158">図 2 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56473-158">See figure 2.</span></span>

<span data-ttu-id="56473-159">Insights API は、[used](/graph/api/resources/insights-used?view=graph-rest-beta) および [shared](/graph/api/resources/insights-shared?view=graph-rest-beta) エンティティと同様の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="56473-159">The insights API provides a similar functionality with the [used](/graph/api/resources/insights-used?view=graph-rest-beta) and [shared](/graph/api/resources/insights-shared?view=graph-rest-beta) entities.</span></span> <span data-ttu-id="56473-160">Office 365 で、あるユーザーが最近表示または操作したもの、または同僚が最近そのユーザーと共有したものが返されます。</span><span class="sxs-lookup"><span data-stu-id="56473-160">They return what a user has been viewing or working on most recently, or what colleagues have shared with the user most recently in Office 365.</span></span>

<span data-ttu-id="56473-161">**図 2 あるユーザーの人物カードが表示されている Outlook on the web**</span><span class="sxs-lookup"><span data-stu-id="56473-161">**Figure 2. Outlook on the web showing a people card for a user**</span></span>

![最近使用したファイルが表示されている、Outlook on the web のあるユーザーの人物カードのスクリーン ショット](images/peoplecard-concept.png)

## <a name="api-reference"></a><span data-ttu-id="56473-163">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="56473-163">API reference</span></span>
<span data-ttu-id="56473-164">これらのサービスの API リファレンスを検索してください。</span><span class="sxs-lookup"><span data-stu-id="56473-164">Looking for the API reference for these services?</span></span>

- [<span data-ttu-id="56473-165">Microsoft ユーザー API は、v1.0 をグラフ化します。</span><span class="sxs-lookup"><span data-stu-id="56473-165">People API in Microsoft Graph v1.0</span></span>](/graph/api/resources/social-overview?view=graph-rest-1.0)
- [<span data-ttu-id="56473-166">社会的知性とベータ版の Microsoft のグラフで分析するための API</span><span class="sxs-lookup"><span data-stu-id="56473-166">API for social intelligence and analytics in Microsoft Graph beta</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="56473-167">次の手順</span><span class="sxs-lookup"><span data-stu-id="56473-167">Next steps</span></span>

* <span data-ttu-id="56473-168">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)を使用して、自分のファイルで People および Insights API を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="56473-168">Use the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out the people and insight APIs with your own files.</span></span> <span data-ttu-id="56473-169">サインインして、左側の列の**サンプルをさらに表示**を選択します。</span><span class="sxs-lookup"><span data-stu-id="56473-169">Sign in, and choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="56473-170">メニューを使用して **People** と **Insights (beta)** を有効にします。</span><span class="sxs-lookup"><span data-stu-id="56473-170">Use the menu to turn on **People** and **Insights (beta)**.</span></span>
* <span data-ttu-id="56473-171">詳細については、[People API](people-example.md) および [person](/graph/api/resources/person?view=graph-rest-1.0) エンティティを参照してください。</span><span class="sxs-lookup"><span data-stu-id="56473-171">Find more about the [people API](people-example.md) and the [person](/graph/api/resources/person?view=graph-rest-1.0) entity.</span></span>
* <span data-ttu-id="56473-172">Insights API を使い始めるには、「[Insights API を使用する](/graph/api/resources/insights?view=graph-rest-beta)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56473-172">To get started with insights API, see [Use the insights API](/graph/api/resources/insights?view=graph-rest-beta).</span></span>
