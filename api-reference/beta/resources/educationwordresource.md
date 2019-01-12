---
title: educationWordResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、Word ドキュメント リソースです。 関連付けられている**fileResource**ディレクトリに Word ファイルをアップロードする必要があります、 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: d67f77774b9d3c428fcfd98006115f0459989fdc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948318"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="19930-105">educationWordResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19930-105">educationWordResource resource type</span></span>

> <span data-ttu-id="19930-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19930-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19930-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19930-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19930-108">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="19930-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="19930-109">これは、Word ドキュメント リソースです。</span><span class="sxs-lookup"><span data-stu-id="19930-109">This is a Word document resource.</span></span> <span data-ttu-id="19930-110">Word ファイルを送信または割り当てに関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="19930-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="19930-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19930-111">Properties</span></span>
| <span data-ttu-id="19930-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19930-112">Property</span></span>     | <span data-ttu-id="19930-113">種類</span><span class="sxs-lookup"><span data-stu-id="19930-113">Type</span></span>   |<span data-ttu-id="19930-114">説明</span><span class="sxs-lookup"><span data-stu-id="19930-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19930-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="19930-115">fileUrl</span></span>|<span data-ttu-id="19930-116">String</span><span class="sxs-lookup"><span data-stu-id="19930-116">String</span></span>|<span data-ttu-id="19930-117">ディスク上のファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="19930-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19930-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19930-118">JSON representation</span></span>

<span data-ttu-id="19930-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19930-119">The following is a JSON representation of the resource.</span></span>

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
