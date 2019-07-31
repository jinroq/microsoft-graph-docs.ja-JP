---
title: " complianceInformation リソースの種類"
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b93e01bf6274591282fd5e486bebb878672d8cc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973231"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="ad4cb-103">complianceInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad4cb-103">complianceInformation resource type</span></span>

<span data-ttu-id="ad4cb-104">セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが保存されています。</span><span class="sxs-lookup"><span data-stu-id="ad4cb-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="ad4cb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad4cb-105">Property</span></span> |<span data-ttu-id="ad4cb-106">型</span><span class="sxs-lookup"><span data-stu-id="ad4cb-106">Type</span></span> |<span data-ttu-id="ad4cb-107">説明</span><span class="sxs-lookup"><span data-stu-id="ad4cb-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ad4cb-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="ad4cb-108">certificationName</span></span> | <span data-ttu-id="ad4cb-109">string</span><span class="sxs-lookup"><span data-stu-id="ad4cb-109">string</span></span> | <span data-ttu-id="ad4cb-110">コンプライアンス証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="ad4cb-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="ad4cb-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="ad4cb-111">certificationControls</span></span> | <span data-ttu-id="ad4cb-112">[certificationControl](certificationcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ad4cb-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="ad4cb-113">証明書に関連付けられている証明書コントロールのコレクション</span><span class="sxs-lookup"><span data-stu-id="ad4cb-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad4cb-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad4cb-114">JSON representation</span></span>

<span data-ttu-id="ad4cb-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad4cb-115">The following is a JSON representation of the resource.</span></span>

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
