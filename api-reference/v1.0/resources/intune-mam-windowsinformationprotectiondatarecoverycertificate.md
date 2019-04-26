---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561188"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="3dd57-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3dd57-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="3dd57-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3dd57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dd57-105">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="3dd57-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="3dd57-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dd57-106">Properties</span></span>
|<span data-ttu-id="3dd57-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dd57-107">Property</span></span>|<span data-ttu-id="3dd57-108">型</span><span class="sxs-lookup"><span data-stu-id="3dd57-108">Type</span></span>|<span data-ttu-id="3dd57-109">説明</span><span class="sxs-lookup"><span data-stu-id="3dd57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dd57-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="3dd57-110">subjectName</span></span>|<span data-ttu-id="3dd57-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3dd57-111">String</span></span>|<span data-ttu-id="3dd57-112">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="3dd57-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="3dd57-113">description</span><span class="sxs-lookup"><span data-stu-id="3dd57-113">description</span></span>|<span data-ttu-id="3dd57-114">String</span><span class="sxs-lookup"><span data-stu-id="3dd57-114">String</span></span>|<span data-ttu-id="3dd57-115">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="3dd57-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="3dd57-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3dd57-116">expirationDateTime</span></span>|<span data-ttu-id="3dd57-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dd57-117">DateTimeOffset</span></span>|<span data-ttu-id="3dd57-118">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="3dd57-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="3dd57-119">certificate</span><span class="sxs-lookup"><span data-stu-id="3dd57-119">certificate</span></span>|<span data-ttu-id="3dd57-120">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="3dd57-120">Binary</span></span>|<span data-ttu-id="3dd57-121">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="3dd57-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dd57-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3dd57-122">Relationships</span></span>
<span data-ttu-id="3dd57-123">なし</span><span class="sxs-lookup"><span data-stu-id="3dd57-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dd57-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3dd57-124">JSON Representation</span></span>
<span data-ttu-id="3dd57-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3dd57-125">Here is a JSON representation of the resource.</span></span>
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



