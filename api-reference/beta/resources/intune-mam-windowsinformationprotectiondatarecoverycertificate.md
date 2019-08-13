---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c3c75af9126c06693b58eb0389c4199092e69c2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373225"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="f23e5-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f23e5-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="f23e5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f23e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f23e5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f23e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23e5-106">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f23e5-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="f23e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f23e5-107">Properties</span></span>
|<span data-ttu-id="f23e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f23e5-108">Property</span></span>|<span data-ttu-id="f23e5-109">型</span><span class="sxs-lookup"><span data-stu-id="f23e5-109">Type</span></span>|<span data-ttu-id="f23e5-110">説明</span><span class="sxs-lookup"><span data-stu-id="f23e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23e5-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="f23e5-111">subjectName</span></span>|<span data-ttu-id="f23e5-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f23e5-112">String</span></span>|<span data-ttu-id="f23e5-113">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="f23e5-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="f23e5-114">description</span><span class="sxs-lookup"><span data-stu-id="f23e5-114">description</span></span>|<span data-ttu-id="f23e5-115">String</span><span class="sxs-lookup"><span data-stu-id="f23e5-115">String</span></span>|<span data-ttu-id="f23e5-116">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="f23e5-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="f23e5-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f23e5-117">expirationDateTime</span></span>|<span data-ttu-id="f23e5-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23e5-118">DateTimeOffset</span></span>|<span data-ttu-id="f23e5-119">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="f23e5-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="f23e5-120">certificate</span><span class="sxs-lookup"><span data-stu-id="f23e5-120">certificate</span></span>|<span data-ttu-id="f23e5-121">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="f23e5-121">Binary</span></span>|<span data-ttu-id="f23e5-122">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="f23e5-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="f23e5-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f23e5-123">Relationships</span></span>
<span data-ttu-id="f23e5-124">なし</span><span class="sxs-lookup"><span data-stu-id="f23e5-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f23e5-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f23e5-125">JSON Representation</span></span>
<span data-ttu-id="f23e5-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f23e5-126">Here is a JSON representation of the resource.</span></span>
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



