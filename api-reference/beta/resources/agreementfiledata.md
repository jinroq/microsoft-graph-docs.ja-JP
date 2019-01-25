---
title: agreementFileData リソースの種類
description: Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517030"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="fc754-103">agreementFileData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc754-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc754-104">Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。</span><span class="sxs-lookup"><span data-stu-id="fc754-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="fc754-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc754-105">Properties</span></span>
| <span data-ttu-id="fc754-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc754-106">Method</span></span>       | <span data-ttu-id="fc754-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fc754-107">Return Type</span></span> | <span data-ttu-id="fc754-108">説明</span><span class="sxs-lookup"><span data-stu-id="fc754-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc754-109">data</span><span class="sxs-lookup"><span data-stu-id="fc754-109">data</span></span>|<span data-ttu-id="fc754-110">Binary</span><span class="sxs-lookup"><span data-stu-id="fc754-110">Binary</span></span>|<span data-ttu-id="fc754-111">PDF 文書の使用の条件を表すデータです。</span><span class="sxs-lookup"><span data-stu-id="fc754-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="fc754-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fc754-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc754-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc754-113">JSON representation</span></span>

<span data-ttu-id="fc754-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fc754-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfiledata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
