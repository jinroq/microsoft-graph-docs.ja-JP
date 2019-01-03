---
title: bitLockerRecoveryOptions リソースの種類
description: BitLocker の回復オプションです。
author: tfitzmac
ms.openlocfilehash: c85ce3111ed88ce8e8bf54c98d5fd3122571a0be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310606"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="fb762-103">bitLockerRecoveryOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb762-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="fb762-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb762-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb762-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb762-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb762-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb762-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb762-107">BitLocker の回復オプションです。</span><span class="sxs-lookup"><span data-stu-id="fb762-107">BitLocker Recovery Options.</span></span>
## <a name="properties"></a><span data-ttu-id="fb762-108">Properties</span><span class="sxs-lookup"><span data-stu-id="fb762-108">Properties</span></span>
|<span data-ttu-id="fb762-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb762-109">Property</span></span>|<span data-ttu-id="fb762-110">種類</span><span class="sxs-lookup"><span data-stu-id="fb762-110">Type</span></span>|<span data-ttu-id="fb762-111">説明</span><span class="sxs-lookup"><span data-stu-id="fb762-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb762-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="fb762-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="fb762-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="fb762-113">Boolean</span></span>|<span data-ttu-id="fb762-114">回復エージェントの証明書ベースのデータをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb762-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="fb762-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="fb762-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="fb762-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="fb762-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="fb762-117">ユーザーの許可または固定の 48 桁の回復パスワードを生成するために必要なのかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="fb762-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="fb762-118">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="fb762-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="fb762-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="fb762-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="fb762-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="fb762-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="fb762-121">ユーザーの許可または固定の 256 ビットの回復キーを生成するために必要なのかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="fb762-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="fb762-122">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="fb762-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="fb762-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="fb762-123">hideRecoveryOptions</span></span>|<span data-ttu-id="fb762-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="fb762-124">Boolean</span></span>|<span data-ttu-id="fb762-125">固定の BitLocker セットアップ ウィザードの回復オプションを表示できるようにするかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="fb762-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="fb762-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="fb762-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="fb762-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="fb762-127">Boolean</span></span>|<span data-ttu-id="fb762-128">AD DS に格納するのには BitLocker 回復情報を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb762-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="fb762-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="fb762-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="fb762-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="fb762-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="fb762-131">どのようなさまざまな BitLocker 回復情報が AD DS に格納されている構成です。</span><span class="sxs-lookup"><span data-stu-id="fb762-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="fb762-132">使用可能な値は、`passwordAndKey`、`passwordOnly` です。</span><span class="sxs-lookup"><span data-stu-id="fb762-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="fb762-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="fb762-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="fb762-134">ブール型</span><span class="sxs-lookup"><span data-stu-id="fb762-134">Boolean</span></span>|<span data-ttu-id="fb762-135">AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb762-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb762-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fb762-136">Relationships</span></span>
<span data-ttu-id="fb762-137">なし</span><span class="sxs-lookup"><span data-stu-id="fb762-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fb762-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb762-138">JSON Representation</span></span>
<span data-ttu-id="fb762-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fb762-139">Here is a JSON representation of the resource.</span></span>
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




