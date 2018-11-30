---
title: educationWordResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、Word ドキュメント リソースです。 関連付けられている**fileResource**ディレクトリに Word ファイルをアップロードする必要があります、 '
ms.openlocfilehash: 28df3278a0d97f440014c342d592d2701b348d94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071868"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="2fcf8-105">educationWordResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fcf8-105">educationWordResource resource type</span></span>

> <span data-ttu-id="2fcf8-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fcf8-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fcf8-108">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2fcf8-109">これは、Word ドキュメント リソースです。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-109">This is a Word document resource.</span></span> <span data-ttu-id="2fcf8-110">Word ファイルを送信または割り当てに関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="2fcf8-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fcf8-111">Properties</span></span>
| <span data-ttu-id="2fcf8-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fcf8-112">Property</span></span>     | <span data-ttu-id="2fcf8-113">型</span><span class="sxs-lookup"><span data-stu-id="2fcf8-113">Type</span></span>   |<span data-ttu-id="2fcf8-114">説明</span><span class="sxs-lookup"><span data-stu-id="2fcf8-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fcf8-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="2fcf8-115">fileUrl</span></span>|<span data-ttu-id="2fcf8-116">String</span><span class="sxs-lookup"><span data-stu-id="2fcf8-116">String</span></span>|<span data-ttu-id="2fcf8-117">ディスク上のファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2fcf8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fcf8-118">JSON representation</span></span>

<span data-ttu-id="2fcf8-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2fcf8-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->