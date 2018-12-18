---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
ms.openlocfilehash: a66c1eeae6d405aa8d0546ac0143e2a8b3404231
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361664"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="58fc5-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58fc5-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="58fc5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="58fc5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58fc5-105">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="58fc5-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="58fc5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58fc5-106">Properties</span></span>
|<span data-ttu-id="58fc5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58fc5-107">Property</span></span>|<span data-ttu-id="58fc5-108">種類</span><span class="sxs-lookup"><span data-stu-id="58fc5-108">Type</span></span>|<span data-ttu-id="58fc5-109">説明</span><span class="sxs-lookup"><span data-stu-id="58fc5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fc5-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="58fc5-110">subjectName</span></span>|<span data-ttu-id="58fc5-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="58fc5-111">String</span></span>|<span data-ttu-id="58fc5-112">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="58fc5-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="58fc5-113">説明</span><span class="sxs-lookup"><span data-stu-id="58fc5-113">description</span></span>|<span data-ttu-id="58fc5-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="58fc5-114">String</span></span>|<span data-ttu-id="58fc5-115">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="58fc5-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="58fc5-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58fc5-116">expirationDateTime</span></span>|<span data-ttu-id="58fc5-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58fc5-117">DateTimeOffset</span></span>|<span data-ttu-id="58fc5-118">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="58fc5-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="58fc5-119">certificate</span><span class="sxs-lookup"><span data-stu-id="58fc5-119">certificate</span></span>|<span data-ttu-id="58fc5-120">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="58fc5-120">Binary</span></span>|<span data-ttu-id="58fc5-121">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="58fc5-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="58fc5-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58fc5-122">Relationships</span></span>
<span data-ttu-id="58fc5-123">なし</span><span class="sxs-lookup"><span data-stu-id="58fc5-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58fc5-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58fc5-124">JSON Representation</span></span>
<span data-ttu-id="58fc5-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58fc5-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



