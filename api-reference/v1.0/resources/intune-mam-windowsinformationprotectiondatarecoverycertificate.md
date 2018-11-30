---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
ms.openlocfilehash: 68faf0e78c68468216c3e69d64926f2c8b18e3c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022821"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="119a8-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="119a8-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="119a8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="119a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="119a8-105">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="119a8-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="119a8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="119a8-106">Properties</span></span>
|<span data-ttu-id="119a8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="119a8-107">Property</span></span>|<span data-ttu-id="119a8-108">型</span><span class="sxs-lookup"><span data-stu-id="119a8-108">Type</span></span>|<span data-ttu-id="119a8-109">説明</span><span class="sxs-lookup"><span data-stu-id="119a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="119a8-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="119a8-110">subjectName</span></span>|<span data-ttu-id="119a8-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="119a8-111">String</span></span>|<span data-ttu-id="119a8-112">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="119a8-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="119a8-113">説明</span><span class="sxs-lookup"><span data-stu-id="119a8-113">description</span></span>|<span data-ttu-id="119a8-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="119a8-114">String</span></span>|<span data-ttu-id="119a8-115">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="119a8-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="119a8-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="119a8-116">expirationDateTime</span></span>|<span data-ttu-id="119a8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119a8-117">DateTimeOffset</span></span>|<span data-ttu-id="119a8-118">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="119a8-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="119a8-119">certificate</span><span class="sxs-lookup"><span data-stu-id="119a8-119">certificate</span></span>|<span data-ttu-id="119a8-120">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="119a8-120">Binary</span></span>|<span data-ttu-id="119a8-121">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="119a8-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="119a8-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="119a8-122">Relationships</span></span>
<span data-ttu-id="119a8-123">なし</span><span class="sxs-lookup"><span data-stu-id="119a8-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="119a8-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="119a8-124">JSON Representation</span></span>
<span data-ttu-id="119a8-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="119a8-125">Here is a JSON representation of the resource.</span></span>
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



