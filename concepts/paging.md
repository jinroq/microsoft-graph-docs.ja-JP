---
title: 'アプリで Microsoft Graph データをページングする '
description: "応答内の、結果の次のページへの URL を含む odata.nextLink' プロパティ。 "
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 6a19d1873057f5a6f6ea1749a6941389b9be8eb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564177"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="fc266-103">アプリで Microsoft Graph データをページングする</span><span class="sxs-lookup"><span data-stu-id="fc266-103">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="fc266-p101">Microsoft Graph に対するクエリの中には、サーバー側のページングを使用したり、1 つの要求におけるページ サイズを限定するために `$top` クエリ パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。要求セットが複数ページにまたがる場合、Microsoft Graph は、結果の次のページへの URL が含まれる `@odata.nextLink` プロパティを応答で返します。</span><span class="sxs-lookup"><span data-stu-id="fc266-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="fc266-106">たとえば、次の URL の場合、組織内のすべてのユーザーのうち、`$top` クエリ パラメーターで指定されたページ サイズ 5 のユーザーを要求します。</span><span class="sxs-lookup"><span data-stu-id="fc266-106">For example, the following URL requests all the users in an organization with a page size of 5, specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="fc266-107">結果に 5 人を超えるユーザーが含まれる場合、Microsoft Graph は、最初のページのユーザーに加えて、次のような `@odata:nextLink` プロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="fc266-107">If the result contains more than five users, Microsoft Graph will return an `@odata:nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="fc266-108">この `@odata:nextLink` プロパティの URL 値を Microsoft Graph に送信することによって、結果の次のページを取得できます。</span><span class="sxs-lookup"><span data-stu-id="fc266-108">You can retrieve the next page of results by sending the URL value of the `@odata:nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="fc266-109">その後、Microsoft Graph はすべての結果ページが読み取られるまで、それぞれの応答の `@odata:nextLink` プロパティ内の次のページのデータへの参照を返します。</span><span class="sxs-lookup"><span data-stu-id="fc266-109">Microsoft Graph will continue to return a reference to the next page of data in the `@odata:nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="fc266-110">**重要:** 結果の次のページの要求には、`@odata:nextLink` プロパティの URL 全体を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc266-110">**Important:** You should include the entire URL in the `@odata:nextLink` property in your request for the next page of results.</span></span> <span data-ttu-id="fc266-111">クエリの実行対象の API によって、`@odata:nextLink` URL 値には `$skiptoken` と `$skip` のいずれかのクエリ パラメーターが入ります。</span><span class="sxs-lookup"><span data-stu-id="fc266-111">Depending on the API that the query is being performed against, the `@odata:nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter.</span></span> <span data-ttu-id="fc266-112">また、URL には、元の要求にある他のクエリ パラメーターすべても含まれます。</span><span class="sxs-lookup"><span data-stu-id="fc266-112">The URL also contains all the other query parameters present in the original request.</span></span> <span data-ttu-id="fc266-113">`$skiptoken` 値または `$skip` 値を抽出して、別の要求で使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="fc266-113">Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="fc266-114">ページング動作は、それぞれの Microsoft Graph API によって異なります。</span><span class="sxs-lookup"><span data-stu-id="fc266-114">Paging behavior varies across different Microsoft Graph APIs.</span></span> <span data-ttu-id="fc266-115">ページングされたデータを扱う場合には、以下の事柄を考慮してください。</span><span class="sxs-lookup"><span data-stu-id="fc266-115">Consider the following when working with paged data:</span></span>

- <span data-ttu-id="fc266-116">API によって、既定および最大のページ サイズが異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="fc266-116">Different APIs might have different default and maximum page sizes.</span></span>
- <span data-ttu-id="fc266-117">(`$top` クエリ パラメーターを使用して) 対象の API の最大ページ サイズを超えるページ サイズを指定する場合には、API によって動作が異なる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fc266-117">Different APIs might behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API.</span></span> <span data-ttu-id="fc266-118">API によっては要求されたページ サイズが無視されることがあります。対象 API の最大ページ サイズに既定で設定されたり、Microsoft Graph によってエラーが返されたりする場合があります。</span><span class="sxs-lookup"><span data-stu-id="fc266-118">Depending on the API, the requested page size might be ignored, it might default to the maximum page size for that API, or Microsoft Graph might return an error.</span></span> 
- <span data-ttu-id="fc266-p105">すべてのリソースまたはリレーションシップでページングがサポートされているわけではありません。たとえば、[directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) に対するクエリではページングはサポートされていません。これにはロール メンバーおよびロール オブジェクト自体の読み取りも含まれます。</span><span class="sxs-lookup"><span data-stu-id="fc266-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) do not support paging. This includes reading role objects themselves as well as role members.</span></span>
