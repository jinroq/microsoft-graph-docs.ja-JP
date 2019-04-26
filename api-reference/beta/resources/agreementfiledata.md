---
title: agreementFileData リソースの種類
description: azure Active Directory (azure AD) 利用規約ファイルの blob を表します。
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339142"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="9cf01-103">agreementFileData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9cf01-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf01-104">azure Active Directory (azure AD) 利用規約ファイルの blob を表します。</span><span class="sxs-lookup"><span data-stu-id="9cf01-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="9cf01-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cf01-105">Properties</span></span>
| <span data-ttu-id="9cf01-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="9cf01-106">Method</span></span>       | <span data-ttu-id="9cf01-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9cf01-107">Return Type</span></span> | <span data-ttu-id="9cf01-108">説明</span><span class="sxs-lookup"><span data-stu-id="9cf01-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9cf01-109">data</span><span class="sxs-lookup"><span data-stu-id="9cf01-109">data</span></span>|<span data-ttu-id="9cf01-110">Binary</span><span class="sxs-lookup"><span data-stu-id="9cf01-110">Binary</span></span>|<span data-ttu-id="9cf01-111">使用条件を表すデータ。 PDF ドキュメント。</span><span class="sxs-lookup"><span data-stu-id="9cf01-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="9cf01-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9cf01-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cf01-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9cf01-113">JSON representation</span></span>

<span data-ttu-id="9cf01-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9cf01-114">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
