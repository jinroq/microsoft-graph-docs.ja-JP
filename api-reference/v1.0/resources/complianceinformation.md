---
title: complianceInformation リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9fc47940b8a9f249e66092ee016453a9eb5152ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032859"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="56c07-103">complianceInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56c07-103">complianceInformation resource type</span></span>

<span data-ttu-id="56c07-104">セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが保存されています。</span><span class="sxs-lookup"><span data-stu-id="56c07-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="56c07-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56c07-105">Properties</span></span>

|<span data-ttu-id="56c07-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56c07-106">Property</span></span> |<span data-ttu-id="56c07-107">型</span><span class="sxs-lookup"><span data-stu-id="56c07-107">Type</span></span> |<span data-ttu-id="56c07-108">説明</span><span class="sxs-lookup"><span data-stu-id="56c07-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="56c07-109">certificationName</span><span class="sxs-lookup"><span data-stu-id="56c07-109">certificationName</span></span>|<span data-ttu-id="56c07-110">String</span><span class="sxs-lookup"><span data-stu-id="56c07-110">String</span></span>| <span data-ttu-id="56c07-111">コンプライアンス証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="56c07-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="56c07-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="56c07-112">certificationControls</span></span>|<span data-ttu-id="56c07-113">[certificationControl](certificationcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="56c07-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="56c07-114">証明書に関連付けられている証明書コントロールのコレクション</span><span class="sxs-lookup"><span data-stu-id="56c07-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56c07-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56c07-115">JSON representation</span></span>

<span data-ttu-id="56c07-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="56c07-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
