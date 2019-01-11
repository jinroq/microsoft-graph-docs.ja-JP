---
title: " complianceInformation リソースの種類"
description: このリソースには、コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820602"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="9f6e6-103">complianceInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f6e6-103">complianceInformation resource type</span></span>

<span data-ttu-id="9f6e6-104">コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="9f6e6-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="9f6e6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f6e6-105">Property</span></span> |<span data-ttu-id="9f6e6-106">種類</span><span class="sxs-lookup"><span data-stu-id="9f6e6-106">Type</span></span> |<span data-ttu-id="9f6e6-107">説明</span><span class="sxs-lookup"><span data-stu-id="9f6e6-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="9f6e6-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="9f6e6-108">certificationName</span></span> | <span data-ttu-id="9f6e6-109">文字列</span><span class="sxs-lookup"><span data-stu-id="9f6e6-109">string</span></span> | <span data-ttu-id="9f6e6-110">コンプライアンスの証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="9f6e6-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="9f6e6-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="9f6e6-111">certificationControls</span></span> | <span data-ttu-id="9f6e6-112">[certificationControl](certificationcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f6e6-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="9f6e6-113">証明書に関連付けられている証明書のコントロールのコレクション</span><span class="sxs-lookup"><span data-stu-id="9f6e6-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f6e6-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f6e6-114">JSON representation</span></span>

<span data-ttu-id="9f6e6-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f6e6-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
