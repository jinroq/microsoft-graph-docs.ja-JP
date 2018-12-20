---
title: " complianceInformation リソースの種類"
description: このリソースには、コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380960"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="e835d-103">complianceInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e835d-103">complianceInformation resource type</span></span>

<span data-ttu-id="e835d-104">コンプライアンスが含まれているに関連付けられているデータは、スコアのコントロールをセキュリティで保護します。</span><span class="sxs-lookup"><span data-stu-id="e835d-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="e835d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e835d-105">Property</span></span> |<span data-ttu-id="e835d-106">型</span><span class="sxs-lookup"><span data-stu-id="e835d-106">Type</span></span> |<span data-ttu-id="e835d-107">説明</span><span class="sxs-lookup"><span data-stu-id="e835d-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="e835d-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="e835d-108">certificationName</span></span> | <span data-ttu-id="e835d-109">文字列</span><span class="sxs-lookup"><span data-stu-id="e835d-109">string</span></span> | <span data-ttu-id="e835d-110">コンプライアンスの証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="e835d-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="e835d-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="e835d-111">certificationControls</span></span> | <span data-ttu-id="e835d-112">[certificationControl](certificationcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e835d-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="e835d-113">証明書に関連付けられている証明書のコントロールのコレクション</span><span class="sxs-lookup"><span data-stu-id="e835d-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e835d-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e835d-114">JSON representation</span></span>

<span data-ttu-id="e835d-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e835d-115">The following is a JSON representation of the resource.</span></span>

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
