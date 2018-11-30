---
title: bitLockerRecoveryOptions リソースの種類
description: BitLocker の回復オプションです。
ms.openlocfilehash: 46af5b52d8305932d0d67ef57d6a1f356182a469
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068536"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="c8955-103">bitLockerRecoveryOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8955-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="c8955-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8955-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8955-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8955-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8955-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8955-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8955-107">BitLocker の回復オプションです。</span><span class="sxs-lookup"><span data-stu-id="c8955-107">BitLocker Recovery Options.</span></span>
## <a name="properties"></a><span data-ttu-id="c8955-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8955-108">Properties</span></span>
|<span data-ttu-id="c8955-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8955-109">Property</span></span>|<span data-ttu-id="c8955-110">型</span><span class="sxs-lookup"><span data-stu-id="c8955-110">Type</span></span>|<span data-ttu-id="c8955-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8955-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8955-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="c8955-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="c8955-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="c8955-113">Boolean</span></span>|<span data-ttu-id="c8955-114">回復エージェントの証明書ベースのデータをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c8955-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="c8955-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="c8955-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="c8955-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c8955-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c8955-117">ユーザーの許可または固定の 48 桁の回復パスワードを生成するために必要なのかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="c8955-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="c8955-118">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="c8955-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c8955-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="c8955-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="c8955-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c8955-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c8955-121">ユーザーの許可または固定の 256 ビットの回復キーを生成するために必要なのかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="c8955-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="c8955-122">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="c8955-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c8955-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="c8955-123">hideRecoveryOptions</span></span>|<span data-ttu-id="c8955-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="c8955-124">Boolean</span></span>|<span data-ttu-id="c8955-125">固定の BitLocker セットアップ ウィザードの回復オプションを表示できるようにするかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="c8955-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="c8955-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="c8955-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="c8955-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="c8955-127">Boolean</span></span>|<span data-ttu-id="c8955-128">AD DS に格納するのには BitLocker 回復情報を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c8955-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="c8955-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="c8955-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="c8955-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="c8955-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="c8955-131">どのようなさまざまな BitLocker 回復情報が AD DS に格納されている構成です。</span><span class="sxs-lookup"><span data-stu-id="c8955-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="c8955-132">使用可能な値は、`passwordAndKey`、`passwordOnly` です。</span><span class="sxs-lookup"><span data-stu-id="c8955-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="c8955-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="c8955-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="c8955-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="c8955-134">Boolean</span></span>|<span data-ttu-id="c8955-135">AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c8955-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8955-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8955-136">Relationships</span></span>
<span data-ttu-id="c8955-137">なし</span><span class="sxs-lookup"><span data-stu-id="c8955-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8955-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8955-138">JSON Representation</span></span>
<span data-ttu-id="c8955-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8955-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```





