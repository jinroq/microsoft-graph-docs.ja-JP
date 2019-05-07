---
title: complianceInformation リソースの種類
description: このリソースには、セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 85fef478a8dcc0f3196355d89f0a20ef0cd7a5b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629307"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="a55c9-103">complianceInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a55c9-103">complianceInformation resource type</span></span>

<span data-ttu-id="a55c9-104">セキュリティで保護されたスコアコントロールに関連するコンプライアンスデータが保存されています。</span><span class="sxs-lookup"><span data-stu-id="a55c9-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="a55c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a55c9-105">Properties</span></span>

|<span data-ttu-id="a55c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a55c9-106">Property</span></span> |<span data-ttu-id="a55c9-107">型</span><span class="sxs-lookup"><span data-stu-id="a55c9-107">Type</span></span> |<span data-ttu-id="a55c9-108">説明</span><span class="sxs-lookup"><span data-stu-id="a55c9-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="a55c9-109">certificationName</span><span class="sxs-lookup"><span data-stu-id="a55c9-109">certificationName</span></span>|<span data-ttu-id="a55c9-110">String</span><span class="sxs-lookup"><span data-stu-id="a55c9-110">String</span></span>| <span data-ttu-id="a55c9-111">コンプライアンス証明書の名前 (たとえば、ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="a55c9-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="a55c9-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="a55c9-112">certificationControls</span></span>|<span data-ttu-id="a55c9-113">[certificationControl](certificationcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a55c9-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="a55c9-114">証明書に関連付けられている証明書コントロールのコレクション</span><span class="sxs-lookup"><span data-stu-id="a55c9-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a55c9-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a55c9-115">JSON representation</span></span>

<span data-ttu-id="a55c9-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a55c9-116">The following is a JSON representation of the resource.</span></span>

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
