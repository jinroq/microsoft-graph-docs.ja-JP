---
title: bitLockerSystemDrivePolicy リソースの種類
description: BitLocker 暗号化の基本ポリシーです。
ms.openlocfilehash: 60388f020750ebd7f187b07777440b013ae5f02a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068914"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="28f8b-103">bitLockerSystemDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28f8b-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="28f8b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28f8b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28f8b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28f8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28f8b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28f8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28f8b-107">BitLocker 暗号化の基本ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="28f8b-107">BitLocker Encryption Base Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="28f8b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f8b-108">Properties</span></span>
|<span data-ttu-id="28f8b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f8b-109">Property</span></span>|<span data-ttu-id="28f8b-110">型</span><span class="sxs-lookup"><span data-stu-id="28f8b-110">Type</span></span>|<span data-ttu-id="28f8b-111">説明</span><span class="sxs-lookup"><span data-stu-id="28f8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28f8b-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="28f8b-112">encryptionMethod</span></span>|[<span data-ttu-id="28f8b-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="28f8b-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="28f8b-114">オペレーティング システム ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="28f8b-115">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="28f8b-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="28f8b-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="28f8b-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="28f8b-117">Boolean</span></span>|<span data-ttu-id="28f8b-118">起動時に追加の認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="28f8b-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="28f8b-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="28f8b-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="28f8b-120">Boolean</span></span>|<span data-ttu-id="28f8b-121">なし (または USB フラッシュ ドライブにスタートアップ キーのパスワードが必要です)、互換性のある TPM は BitLocker を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="28f8b-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="28f8b-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="28f8b-124">TPM スタートアップを許可または必要と許可しないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="28f8b-125">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="28f8b-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="28f8b-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="28f8b-128">TPM スタートアップの暗証番号 (pin) を許可または必要と許可しないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="28f8b-129">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="28f8b-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="28f8b-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="28f8b-132">スタートアップ キーを TPM を許可または必要と許可しないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="28f8b-133">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="28f8b-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="28f8b-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="28f8b-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="28f8b-136">TPM スタートアップに追加することを示しますキーとキーは、許可または必要と許可しません。</span><span class="sxs-lookup"><span data-stu-id="28f8b-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="28f8b-137">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="28f8b-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="28f8b-138">minimumPinLength</span></span>|<span data-ttu-id="28f8b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="28f8b-139">Int32</span></span>|<span data-ttu-id="28f8b-140">スタートアップの暗証番号 (pin) の最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="28f8b-141">4 ~ 20 の有効な値</span><span class="sxs-lookup"><span data-stu-id="28f8b-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="28f8b-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="28f8b-142">recoveryOptions</span></span>|[<span data-ttu-id="28f8b-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="28f8b-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="28f8b-144">必要なスタートアップ キー情報がない場合、BitLocker で暗号化されたオペレーティング システム ドライブを回復することができます。</span><span class="sxs-lookup"><span data-stu-id="28f8b-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="28f8b-145">BitLocker を有効にするときは、このポリシー設定が適用されます。</span><span class="sxs-lookup"><span data-stu-id="28f8b-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="28f8b-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="28f8b-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="28f8b-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="28f8b-147">Boolean</span></span>|<span data-ttu-id="28f8b-148">ブート前の回復のメッセージと Url を有効にします。</span><span class="sxs-lookup"><span data-stu-id="28f8b-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="28f8b-149">RequireStartupAuthentication が false の場合、この値は影響しません。</span><span class="sxs-lookup"><span data-stu-id="28f8b-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="28f8b-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="28f8b-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="28f8b-151">String</span><span class="sxs-lookup"><span data-stu-id="28f8b-151">String</span></span>|<span data-ttu-id="28f8b-152">回復のカスタム メッセージを定義します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="28f8b-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="28f8b-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="28f8b-154">String</span><span class="sxs-lookup"><span data-stu-id="28f8b-154">String</span></span>|<span data-ttu-id="28f8b-155">回復のカスタム URL を定義します。</span><span class="sxs-lookup"><span data-stu-id="28f8b-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28f8b-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28f8b-156">Relationships</span></span>
<span data-ttu-id="28f8b-157">なし</span><span class="sxs-lookup"><span data-stu-id="28f8b-157">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28f8b-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28f8b-158">JSON Representation</span></span>
<span data-ttu-id="28f8b-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28f8b-159">Here is a JSON representation of the resource.</span></span>
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





