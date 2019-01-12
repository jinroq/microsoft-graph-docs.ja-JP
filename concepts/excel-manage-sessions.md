---
title: Microsoft Graph によって Excel のセッションと永続化を管理する
description: アプリケーションで Excel API の呼び出しを 1 回以上行う必要がある場合は、セッションを作成し、要求ごとにセッション ID を渡す必要がります。 要求にセッション ID を含めると、Excel API を最も効率的な方法で使用できるようになります。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 151119a2a2861b64db126c8f49d0b916a6f563e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921690"
---
# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a><span data-ttu-id="5f034-104">Microsoft Graph によって Excel のセッションと永続化を管理する</span><span class="sxs-lookup"><span data-stu-id="5f034-104">Manage sessions and persistence in Excel with Microsoft Graph</span></span>

<span data-ttu-id="5f034-105">アプリケーションで Excel API の呼び出しを 1 回以上行う必要がある場合は、セッションを作成し、要求ごとにセッション ID を渡す必要がります。</span><span class="sxs-lookup"><span data-stu-id="5f034-105">If your application needs to make more than one or two calls to the Excel API, you should create a session and pass the session Id with each request.</span></span> <span data-ttu-id="5f034-106">要求にセッション ID を含めると、Excel API を最も効率的な方法で使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="5f034-106">The presence of a session Id in the requests ensures that you are using the Excel API in the most efficient way possible.</span></span>

<span data-ttu-id="5f034-107">Excel API は、次の 3 つのモードのいずれかで呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="5f034-107">Excel APIs are called in one of three modes:</span></span>

1. <span data-ttu-id="5f034-108">**永続セッション**: ブックに加えられたすべての変更がブックに永続化 (保存) されます。</span><span class="sxs-lookup"><span data-stu-id="5f034-108">**Persistent session**  All changes made to the workbook are persisted (saved) to the workbook.</span></span> <span data-ttu-id="5f034-109">これは、最も効率的でパフォーマンスの高い Excel API の使用方法です。</span><span class="sxs-lookup"><span data-stu-id="5f034-109">This is the most efficient and best-performing way to use the Excel API.</span></span>
2. <span data-ttu-id="5f034-110">**非永続セッション**: API によって加えられた変更は元の場所に保存されません。</span><span class="sxs-lookup"><span data-stu-id="5f034-110">**Non-persistent session**  Changes made by the API are not saved to the source location.</span></span> <span data-ttu-id="5f034-111">代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。</span><span class="sxs-lookup"><span data-stu-id="5f034-111">Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session.</span></span> <span data-ttu-id="5f034-112">Excel のセッションの有効期限が切れると、変更は失われます。</span><span class="sxs-lookup"><span data-stu-id="5f034-112">When the Excel session expires, the changes are lost.</span></span> <span data-ttu-id="5f034-113">分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるが、ドキュメントの状態に影響を与える必要がないアプリでは、このモードが便利です。</span><span class="sxs-lookup"><span data-stu-id="5f034-113">This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but do not need to affect the document state.</span></span>
3. <span data-ttu-id="5f034-114">**セッションレス**: API の呼び出しでセッション ID を渡しません。Excel サーバーは、操作ごとにサーバーに保存されたブックのコピーを検索する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f034-114">**Sessionless**  The API calls do not pass a session Id. The Excel servers have to locate the server's copy of the workbook for each operation.</span></span> <span data-ttu-id="5f034-115">これは、効率的な Excel API の呼び出し方法ではありませんが、ある種の独立した要求を行うのに適しています。</span><span class="sxs-lookup"><span data-stu-id="5f034-115">This is not an efficient way to call the Excel API, but it is suitable for making certain types of isolated requests.</span></span>

<span data-ttu-id="5f034-116">API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="5f034-116">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span>

><span data-ttu-id="5f034-p106">**注:** セッション ヘッダーは Excel API が機能するために必要ではありません。しかし、パフォーマンスを向上させるためにセッション ヘッダーを使用することをお勧めします。セッション ヘッダーを使用しない場合は、API の呼び出し時に行われた変更がファイルに永続化_されます_。</span><span class="sxs-lookup"><span data-stu-id="5f034-p106">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="next-step"></a><span data-ttu-id="5f034-120">次のステップ</span><span class="sxs-lookup"><span data-stu-id="5f034-120">Next step</span></span>
<span data-ttu-id="5f034-121">セッションの作成方法と使用方法については、[セッション作成のリファレンス トピック](/graph/api/workbook-createsession?view=graph-rest-1.0)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f034-121">To learn how to create and use sessions, see the [Create session reference topic](/graph/api/workbook-createsession?view=graph-rest-1.0).</span></span>

## <a name="see-also"></a><span data-ttu-id="5f034-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f034-122">See also</span></span>
* [<span data-ttu-id="5f034-123">Microsoft Graph を使用して Excel ブックに書き込む</span><span class="sxs-lookup"><span data-stu-id="5f034-123">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="5f034-124">Microsoft Graph で Excel のブック関数を使用する</span><span class="sxs-lookup"><span data-stu-id="5f034-124">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="5f034-125">Microsoft Graph により Excel のある範囲の書式を更新する</span><span class="sxs-lookup"><span data-stu-id="5f034-125">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="5f034-126">Microsoft Graph により Excel のグラフ イメージを表示する</span><span class="sxs-lookup"><span data-stu-id="5f034-126">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="5f034-127">Excel REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="5f034-127">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
