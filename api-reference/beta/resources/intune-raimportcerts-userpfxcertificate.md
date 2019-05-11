---
title: userPFXCertificate リソースの種類
description: ユーザーの PFX 証明書に必要なすべての情報をカプセル化するエンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9c4af075d026c036b31ac9083ff05aec07b0bb6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940065"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="aede1-103">userPFXCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aede1-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="aede1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aede1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aede1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aede1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aede1-106">ユーザーの PFX 証明書に必要なすべての情報をカプセル化するエンティティ。</span><span class="sxs-lookup"><span data-stu-id="aede1-106">Entity that encapsulates all information required for a user's PFX certificates.</span></span>

## <a name="methods"></a><span data-ttu-id="aede1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="aede1-107">Methods</span></span>
|<span data-ttu-id="aede1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="aede1-108">Method</span></span>|<span data-ttu-id="aede1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aede1-109">Return Type</span></span>|<span data-ttu-id="aede1-110">説明</span><span class="sxs-lookup"><span data-stu-id="aede1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aede1-111">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="aede1-111">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="aede1-112">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aede1-112">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="aede1-113">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="aede1-113">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="aede1-114">UserPFXCertificate を取得する</span><span class="sxs-lookup"><span data-stu-id="aede1-114">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="aede1-115">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="aede1-115">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="aede1-116">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aede1-116">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="aede1-117">UserPFXCertificate を作成する</span><span class="sxs-lookup"><span data-stu-id="aede1-117">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="aede1-118">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="aede1-118">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="aede1-119">新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="aede1-119">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="aede1-120">UserPFXCertificate の削除</span><span class="sxs-lookup"><span data-stu-id="aede1-120">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="aede1-121">None</span><span class="sxs-lookup"><span data-stu-id="aede1-121">None</span></span>|<span data-ttu-id="aede1-122">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="aede1-122">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="aede1-123">UserPFXCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="aede1-123">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="aede1-124">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="aede1-124">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="aede1-125">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aede1-125">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aede1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aede1-126">Properties</span></span>
|<span data-ttu-id="aede1-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aede1-127">Property</span></span>|<span data-ttu-id="aede1-128">型</span><span class="sxs-lookup"><span data-stu-id="aede1-128">Type</span></span>|<span data-ttu-id="aede1-129">説明</span><span class="sxs-lookup"><span data-stu-id="aede1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aede1-130">id</span><span class="sxs-lookup"><span data-stu-id="aede1-130">id</span></span>|<span data-ttu-id="aede1-131">文字列</span><span class="sxs-lookup"><span data-stu-id="aede1-131">String</span></span>|<span data-ttu-id="aede1-132">PFX 証明書の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="aede1-132">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="aede1-133">拇印</span><span class="sxs-lookup"><span data-stu-id="aede1-133">thumbprint</span></span>|<span data-ttu-id="aede1-134">String</span><span class="sxs-lookup"><span data-stu-id="aede1-134">String</span></span>|<span data-ttu-id="aede1-135">PFX 証明書の SHA-1 拇印。</span><span class="sxs-lookup"><span data-stu-id="aede1-135">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="aede1-136">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="aede1-136">intendedPurpose</span></span>|[<span data-ttu-id="aede1-137">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="aede1-137">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="aede1-138">展開の観点から見た証明書の目的。</span><span class="sxs-lookup"><span data-stu-id="aede1-138">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="aede1-139">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="aede1-139">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="aede1-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aede1-140">userPrincipalName</span></span>|<span data-ttu-id="aede1-141">String</span><span class="sxs-lookup"><span data-stu-id="aede1-141">String</span></span>|<span data-ttu-id="aede1-142">PFX 証明書のユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="aede1-142">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="aede1-143">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aede1-143">startDateTime</span></span>|<span data-ttu-id="aede1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aede1-144">DateTimeOffset</span></span>|<span data-ttu-id="aede1-145">証明書の有効期間の開始日/時刻。</span><span class="sxs-lookup"><span data-stu-id="aede1-145">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="aede1-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aede1-146">expirationDateTime</span></span>|<span data-ttu-id="aede1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aede1-147">DateTimeOffset</span></span>|<span data-ttu-id="aede1-148">証明書の有効期限の日付/時刻。</span><span class="sxs-lookup"><span data-stu-id="aede1-148">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="aede1-149">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="aede1-149">providerName</span></span>|<span data-ttu-id="aede1-150">String</span><span class="sxs-lookup"><span data-stu-id="aede1-150">String</span></span>|<span data-ttu-id="aede1-151">この blob を暗号化するために使用される暗号化プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="aede1-151">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="aede1-152">keyName</span><span class="sxs-lookup"><span data-stu-id="aede1-152">keyName</span></span>|<span data-ttu-id="aede1-153">String</span><span class="sxs-lookup"><span data-stu-id="aede1-153">String</span></span>|<span data-ttu-id="aede1-154">Blob の暗号化に使用された (プロバイダー内の) キーの名前。</span><span class="sxs-lookup"><span data-stu-id="aede1-154">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="aede1-155">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="aede1-155">paddingScheme</span></span>|[<span data-ttu-id="aede1-156">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="aede1-156">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="aede1-157">暗号化/復号化時にプロバイダーによって使用されるパディング方式。</span><span class="sxs-lookup"><span data-stu-id="aede1-157">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="aede1-158">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="aede1-158">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="aede1-159">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="aede1-159">encryptedPfxBlob</span></span>|<span data-ttu-id="aede1-160">Binary</span><span class="sxs-lookup"><span data-stu-id="aede1-160">Binary</span></span>|<span data-ttu-id="aede1-161">暗号化された PFX blob。</span><span class="sxs-lookup"><span data-stu-id="aede1-161">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="aede1-162">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="aede1-162">encryptedPfxPassword</span></span>|<span data-ttu-id="aede1-163">String</span><span class="sxs-lookup"><span data-stu-id="aede1-163">String</span></span>|<span data-ttu-id="aede1-164">暗号化された PFX パスワード。</span><span class="sxs-lookup"><span data-stu-id="aede1-164">Encrypted PFX password.</span></span>|
|<span data-ttu-id="aede1-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aede1-165">createdDateTime</span></span>|<span data-ttu-id="aede1-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aede1-166">DateTimeOffset</span></span>|<span data-ttu-id="aede1-167">この PFX 証明書がインポートされた日付/時刻です。</span><span class="sxs-lookup"><span data-stu-id="aede1-167">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="aede1-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aede1-168">lastModifiedDateTime</span></span>|<span data-ttu-id="aede1-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aede1-169">DateTimeOffset</span></span>|<span data-ttu-id="aede1-170">この PFX 証明書が最後に変更された日付/時刻。</span><span class="sxs-lookup"><span data-stu-id="aede1-170">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aede1-171">関係</span><span class="sxs-lookup"><span data-stu-id="aede1-171">Relationships</span></span>
<span data-ttu-id="aede1-172">なし</span><span class="sxs-lookup"><span data-stu-id="aede1-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aede1-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aede1-173">JSON Representation</span></span>
<span data-ttu-id="aede1-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aede1-174">Here is a JSON representation of the resource.</span></span>
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




