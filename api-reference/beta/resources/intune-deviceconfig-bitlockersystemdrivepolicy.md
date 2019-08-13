---
title: Bitlockersystemdrive Policy リソースの種類
description: BitLocker 暗号化の基本ポリシー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4ffeaca0d5ee305690c05337eeb75787ece9641
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333766"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="e18ba-103">Bitlockersystemdrive Policy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e18ba-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="e18ba-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e18ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e18ba-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e18ba-106">BitLocker 暗号化の基本ポリシー。</span><span class="sxs-lookup"><span data-stu-id="e18ba-106">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="e18ba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e18ba-107">Properties</span></span>
|<span data-ttu-id="e18ba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e18ba-108">Property</span></span>|<span data-ttu-id="e18ba-109">型</span><span class="sxs-lookup"><span data-stu-id="e18ba-109">Type</span></span>|<span data-ttu-id="e18ba-110">説明</span><span class="sxs-lookup"><span data-stu-id="e18ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e18ba-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e18ba-111">encryptionMethod</span></span>|[<span data-ttu-id="e18ba-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e18ba-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="e18ba-113">オペレーティングシステムドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-113">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="e18ba-114">使用可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="e18ba-115">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="e18ba-115">startupAuthenticationRequired</span></span>|<span data-ttu-id="e18ba-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18ba-116">Boolean</span></span>|<span data-ttu-id="e18ba-117">起動時に追加の認証を要求します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-117">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="e18ba-118">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="e18ba-118">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="e18ba-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18ba-119">Boolean</span></span>|<span data-ttu-id="e18ba-120">互換性のある TPM を使用せずに BitLocker を許可するかどうかを示します (パスワードまたは USB フラッシュドライブのスタートアップキーが必要です)。</span><span class="sxs-lookup"><span data-stu-id="e18ba-120">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="e18ba-121">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-121">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="e18ba-122">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-122">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e18ba-123">TPM のスタートアップが許可されているかどうか、または要求/禁止を示します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-123">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="e18ba-124">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-124">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e18ba-125">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-125">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="e18ba-126">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-126">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e18ba-127">TPM スタートアップ pin が許可されているかどうか、または許可/禁止を示します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-127">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="e18ba-128">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-128">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e18ba-129">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-129">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="e18ba-130">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-130">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e18ba-131">TPM スタートアップキーが許可されているかどうか、または必要/不許可かを示します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-131">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="e18ba-132">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-132">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e18ba-133">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-133">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="e18ba-134">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e18ba-134">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e18ba-135">TPM スタートアップ pin キーとキーが許可されているかどうか、または許可/不許可かを示します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-135">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="e18ba-136">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-136">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e18ba-137">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="e18ba-137">minimumPinLength</span></span>|<span data-ttu-id="e18ba-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e18ba-138">Int32</span></span>|<span data-ttu-id="e18ba-139">スタートアップ pin の最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-139">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="e18ba-140">有効な値は4から20までです</span><span class="sxs-lookup"><span data-stu-id="e18ba-140">Valid values 4 to 20</span></span>|
|<span data-ttu-id="e18ba-141">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="e18ba-141">recoveryOptions</span></span>|[<span data-ttu-id="e18ba-142">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="e18ba-142">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="e18ba-143">必要なスタートアップキー情報がない場合に BitLocker で暗号化されたオペレーティングシステムドライブを回復できるようにします。</span><span class="sxs-lookup"><span data-stu-id="e18ba-143">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="e18ba-144">このポリシー設定は、BitLocker を有効にしたときに適用されます。</span><span class="sxs-lookup"><span data-stu-id="e18ba-144">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="e18ba-145">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="e18ba-145">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="e18ba-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18ba-146">Boolean</span></span>|<span data-ttu-id="e18ba-147">ブート前の回復メッセージと Url を有効にします。</span><span class="sxs-lookup"><span data-stu-id="e18ba-147">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="e18ba-148">RequireStartupAuthentication が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="e18ba-148">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="e18ba-149">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="e18ba-149">prebootRecoveryMessage</span></span>|<span data-ttu-id="e18ba-150">String</span><span class="sxs-lookup"><span data-stu-id="e18ba-150">String</span></span>|<span data-ttu-id="e18ba-151">カスタムの回復メッセージを定義します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-151">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="e18ba-152">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="e18ba-152">prebootRecoveryUrl</span></span>|<span data-ttu-id="e18ba-153">String</span><span class="sxs-lookup"><span data-stu-id="e18ba-153">String</span></span>|<span data-ttu-id="e18ba-154">カスタムの回復 URL を定義します。</span><span class="sxs-lookup"><span data-stu-id="e18ba-154">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e18ba-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e18ba-155">Relationships</span></span>
<span data-ttu-id="e18ba-156">なし</span><span class="sxs-lookup"><span data-stu-id="e18ba-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e18ba-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e18ba-157">JSON Representation</span></span>
<span data-ttu-id="e18ba-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e18ba-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```



