---
title: インサイト リソースの種類
description: インサイトとは、高度な分析と機械学習の機能を使って計算されるリレーションシップのことです。 たとえば、ユーザーの周囲で人気急上昇中の OneDrive ドキュメントを特定することができます。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640169"
---
# <a name="insights-resource-type"></a><span data-ttu-id="70c17-104">インサイト リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70c17-104">insights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70c17-105">インサイトとは、高度な分析と機械学習の機能を使って計算されるリレーションシップのことです。</span><span class="sxs-lookup"><span data-stu-id="70c17-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="70c17-106">たとえば、ユーザーの周囲で人気急上昇中の OneDrive ドキュメントを特定することができます。</span><span class="sxs-lookup"><span data-stu-id="70c17-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="70c17-107">インサイトは、次の API によって返されます。</span><span class="sxs-lookup"><span data-stu-id="70c17-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="70c17-108">[Trending](insights-trending.md) - ユーザーの周囲で人気上昇中の OneDrive ドキュメントや SharePoint サイトを返します。</span><span class="sxs-lookup"><span data-stu-id="70c17-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="70c17-109">[Used](insights-used.md) - ユーザーが表示および変更したドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="70c17-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="70c17-110">ユーザーが OneDrive for Business、SharePoint で使ったドキュメント、メールの添付ファイルとして、あるいは Box、DropBox、Google ドライブなどのソースからのリンクの添付ファイルとして開いたドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70c17-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="70c17-111">[Shared](insights-shared.md) - ユーザーと共有されているドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="70c17-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="70c17-112">ドキュメントは、メールの添付ファイルとして、またはメールで送信した OneDrive for Business のリンクとして共有できます。</span><span class="sxs-lookup"><span data-stu-id="70c17-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="70c17-113">各インサイトは、`resourceVisualization` と `resourceReference` の複合値型 (CVT) で返されます。</span><span class="sxs-lookup"><span data-stu-id="70c17-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="70c17-114">resourceVisualization CVT には `title` と `previewImageUrl` などのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70c17-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="70c17-115">Microsoft では、視覚化プロパティを使って Office Delve のようなエクスペリエンスでファイルをレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="70c17-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="70c17-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70c17-116">Relationships</span></span>

| <span data-ttu-id="70c17-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70c17-117">Relationship</span></span>      | <span data-ttu-id="70c17-118">型</span><span class="sxs-lookup"><span data-stu-id="70c17-118">Type</span></span>          | <span data-ttu-id="70c17-119">説明</span><span class="sxs-lookup"><span data-stu-id="70c17-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="70c17-120">trending</span><span class="sxs-lookup"><span data-stu-id="70c17-120">trending</span></span>      | <span data-ttu-id="70c17-121">[Trending](insights-trending.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="70c17-121">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="70c17-122">計算されたリレーションシップによって人気上昇中のドキュメントを識別します。</span><span class="sxs-lookup"><span data-stu-id="70c17-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="70c17-123">人気上昇中のドキュメントは、OneDrive または SharePoint のサイトに保存することができます。</span><span class="sxs-lookup"><span data-stu-id="70c17-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="70c17-124">used</span><span class="sxs-lookup"><span data-stu-id="70c17-124">used</span></span>      | <span data-ttu-id="70c17-125">[Used](insights-used.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="70c17-125">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="70c17-126">計算されたリレーションシップによってユーザーが表示したり変更したりしたドキュメントを識別します。</span><span class="sxs-lookup"><span data-stu-id="70c17-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="70c17-127">ユーザーが OneDrive for Business、SharePoint で使ったドキュメント、メールの添付ファイルとして、あるいは Box、DropBox、Google ドライブなどのソースからのリンクの添付ファイルとして開いたドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70c17-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="70c17-128">shared</span><span class="sxs-lookup"><span data-stu-id="70c17-128">shared</span></span>        | <span data-ttu-id="70c17-129">[Shared](insights-shared.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="70c17-129">[shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="70c17-130">計算されたリレーションシップによってユーザーが共有しているドキュメントを識別します。</span><span class="sxs-lookup"><span data-stu-id="70c17-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="70c17-131">ドキュメントは、メールの添付ファイルとして、またはメールで送信した OneDrive for Business のリンクとして共有できます。</span><span class="sxs-lookup"><span data-stu-id="70c17-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="70c17-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70c17-132">JSON representation</span></span>

<span data-ttu-id="70c17-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="70c17-133">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
