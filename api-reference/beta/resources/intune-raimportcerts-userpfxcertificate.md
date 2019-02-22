---
title: userPFXCertificate リソースの種類
description: ユーザーの PFX 証明書に必要なすべての情報をカプセル化するエンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 534b2fa0f5f3240ead38deae45d3cc88091e40d8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154930"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="cf687-103">userPFXCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf687-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="cf687-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf687-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf687-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf687-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf687-106">ユーザーの PFX 証明書に必要なすべての情報をカプセル化するエンティティ。</span><span class="sxs-lookup"><span data-stu-id="cf687-106">Entity that encapsulates all information required for a user's PFX certificates.</span></span>

## <a name="methods"></a><span data-ttu-id="cf687-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf687-107">Methods</span></span>
|<span data-ttu-id="cf687-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf687-108">Method</span></span>|<span data-ttu-id="cf687-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cf687-109">Return Type</span></span>|<span data-ttu-id="cf687-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf687-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf687-111">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="cf687-111">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="cf687-112">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cf687-112">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="cf687-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cf687-113">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="cf687-114">userPFXCertificate を取得する</span><span class="sxs-lookup"><span data-stu-id="cf687-114">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="cf687-115">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="cf687-115">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="cf687-116">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cf687-116">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="cf687-117">userPFXCertificate を作成する</span><span class="sxs-lookup"><span data-stu-id="cf687-117">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="cf687-118">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="cf687-118">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="cf687-119">新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf687-119">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="cf687-120">userPFXCertificate の削除</span><span class="sxs-lookup"><span data-stu-id="cf687-120">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="cf687-121">なし</span><span class="sxs-lookup"><span data-stu-id="cf687-121">None</span></span>|<span data-ttu-id="cf687-122">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="cf687-122">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="cf687-123">userPFXCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="cf687-123">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="cf687-124">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="cf687-124">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="cf687-125">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cf687-125">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf687-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf687-126">Properties</span></span>
|<span data-ttu-id="cf687-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf687-127">Property</span></span>|<span data-ttu-id="cf687-128">型</span><span class="sxs-lookup"><span data-stu-id="cf687-128">Type</span></span>|<span data-ttu-id="cf687-129">説明</span><span class="sxs-lookup"><span data-stu-id="cf687-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf687-130">id</span><span class="sxs-lookup"><span data-stu-id="cf687-130">id</span></span>|<span data-ttu-id="cf687-131">String</span><span class="sxs-lookup"><span data-stu-id="cf687-131">String</span></span>|<span data-ttu-id="cf687-132">PFX 証明書の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cf687-132">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="cf687-133">拇印</span><span class="sxs-lookup"><span data-stu-id="cf687-133">thumbprint</span></span>|<span data-ttu-id="cf687-134">String</span><span class="sxs-lookup"><span data-stu-id="cf687-134">String</span></span>|<span data-ttu-id="cf687-135">PFX 証明書の sha-1 拇印。</span><span class="sxs-lookup"><span data-stu-id="cf687-135">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="cf687-136">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="cf687-136">intendedPurpose</span></span>|[<span data-ttu-id="cf687-137">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="cf687-137">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="cf687-138">展開の観点から見た証明書の目的。</span><span class="sxs-lookup"><span data-stu-id="cf687-138">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="cf687-139">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="cf687-139">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="cf687-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf687-140">userPrincipalName</span></span>|<span data-ttu-id="cf687-141">String</span><span class="sxs-lookup"><span data-stu-id="cf687-141">String</span></span>|<span data-ttu-id="cf687-142">PFX 証明書のユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="cf687-142">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="cf687-143">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cf687-143">startDateTime</span></span>|<span data-ttu-id="cf687-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf687-144">DateTimeOffset</span></span>|<span data-ttu-id="cf687-145">証明書の有効期間の開始日/時刻。</span><span class="sxs-lookup"><span data-stu-id="cf687-145">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="cf687-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cf687-146">expirationDateTime</span></span>|<span data-ttu-id="cf687-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf687-147">DateTimeOffset</span></span>|<span data-ttu-id="cf687-148">証明書の有効期限の日付/時刻。</span><span class="sxs-lookup"><span data-stu-id="cf687-148">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="cf687-149">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="cf687-149">providerName</span></span>|<span data-ttu-id="cf687-150">String</span><span class="sxs-lookup"><span data-stu-id="cf687-150">String</span></span>|<span data-ttu-id="cf687-151">この blob を暗号化するために使用される暗号化プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="cf687-151">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="cf687-152">keyName</span><span class="sxs-lookup"><span data-stu-id="cf687-152">keyName</span></span>|<span data-ttu-id="cf687-153">String</span><span class="sxs-lookup"><span data-stu-id="cf687-153">String</span></span>|<span data-ttu-id="cf687-154">blob の暗号化に使用された (プロバイダー内の) キーの名前。</span><span class="sxs-lookup"><span data-stu-id="cf687-154">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="cf687-155">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="cf687-155">paddingScheme</span></span>|[<span data-ttu-id="cf687-156">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="cf687-156">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="cf687-157">暗号化/復号化時にプロバイダーによって使用されるパディング方式。</span><span class="sxs-lookup"><span data-stu-id="cf687-157">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="cf687-158">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="cf687-158">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="cf687-159">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="cf687-159">encryptedPfxBlob</span></span>|<span data-ttu-id="cf687-160">Binary</span><span class="sxs-lookup"><span data-stu-id="cf687-160">Binary</span></span>|<span data-ttu-id="cf687-161">暗号化された PFX blob。</span><span class="sxs-lookup"><span data-stu-id="cf687-161">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="cf687-162">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="cf687-162">encryptedPfxPassword</span></span>|<span data-ttu-id="cf687-163">String</span><span class="sxs-lookup"><span data-stu-id="cf687-163">String</span></span>|<span data-ttu-id="cf687-164">暗号化された PFX パスワード。</span><span class="sxs-lookup"><span data-stu-id="cf687-164">Encrypted PFX password.</span></span>|
|<span data-ttu-id="cf687-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf687-165">createdDateTime</span></span>|<span data-ttu-id="cf687-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf687-166">DateTimeOffset</span></span>|<span data-ttu-id="cf687-167">この PFX 証明書がインポートされた日付/時刻です。</span><span class="sxs-lookup"><span data-stu-id="cf687-167">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="cf687-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf687-168">lastModifiedDateTime</span></span>|<span data-ttu-id="cf687-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf687-169">DateTimeOffset</span></span>|<span data-ttu-id="cf687-170">この PFX 証明書が最後に変更された日付/時刻。</span><span class="sxs-lookup"><span data-stu-id="cf687-170">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf687-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf687-171">Relationships</span></span>
<span data-ttu-id="cf687-172">なし</span><span class="sxs-lookup"><span data-stu-id="cf687-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf687-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf687-173">JSON Representation</span></span>
<span data-ttu-id="cf687-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf687-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




