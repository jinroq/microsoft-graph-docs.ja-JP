---
title: userPFXCertificate リソースの種類
description: PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 95ae97b44a82d5ec87e3e2622a519debcfd8d7c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406039"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="15606-103">userPFXCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15606-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="15606-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15606-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15606-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15606-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15606-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15606-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15606-107">PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="15606-107">Entity that encapsulates all information required for a user's PFX certificates.</span></span>

## <a name="methods"></a><span data-ttu-id="15606-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="15606-108">Methods</span></span>
|<span data-ttu-id="15606-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="15606-109">Method</span></span>|<span data-ttu-id="15606-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="15606-110">Return Type</span></span>|<span data-ttu-id="15606-111">説明</span><span class="sxs-lookup"><span data-stu-id="15606-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15606-112">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="15606-112">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="15606-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="15606-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="15606-114">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="15606-114">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="15606-115">UserPFXCertificate を取得します。</span><span class="sxs-lookup"><span data-stu-id="15606-115">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="15606-116">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="15606-116">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="15606-117">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15606-117">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="15606-118">UserPFXCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="15606-118">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="15606-119">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="15606-119">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="15606-120">新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="15606-120">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="15606-121">UserPFXCertificate を削除します。</span><span class="sxs-lookup"><span data-stu-id="15606-121">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="15606-122">なし</span><span class="sxs-lookup"><span data-stu-id="15606-122">None</span></span>|<span data-ttu-id="15606-123">の[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="15606-123">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="15606-124">UserPFXCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="15606-124">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="15606-125">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="15606-125">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="15606-126">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15606-126">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15606-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15606-127">Properties</span></span>
|<span data-ttu-id="15606-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15606-128">Property</span></span>|<span data-ttu-id="15606-129">型</span><span class="sxs-lookup"><span data-stu-id="15606-129">Type</span></span>|<span data-ttu-id="15606-130">説明</span><span class="sxs-lookup"><span data-stu-id="15606-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15606-131">id</span><span class="sxs-lookup"><span data-stu-id="15606-131">id</span></span>|<span data-ttu-id="15606-132">String</span><span class="sxs-lookup"><span data-stu-id="15606-132">String</span></span>|<span data-ttu-id="15606-133">PFX 証明書の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="15606-133">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="15606-134">拇印</span><span class="sxs-lookup"><span data-stu-id="15606-134">thumbprint</span></span>|<span data-ttu-id="15606-135">String</span><span class="sxs-lookup"><span data-stu-id="15606-135">String</span></span>|<span data-ttu-id="15606-136">PFX 証明書の拇印を sha-1 です。</span><span class="sxs-lookup"><span data-stu-id="15606-136">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="15606-137">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="15606-137">intendedPurpose</span></span>|[<span data-ttu-id="15606-138">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="15606-138">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="15606-139">証明書からのポイントからのビューの展開の目的のものです。</span><span class="sxs-lookup"><span data-stu-id="15606-139">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="15606-140">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="15606-140">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="15606-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="15606-141">userPrincipalName</span></span>|<span data-ttu-id="15606-142">String</span><span class="sxs-lookup"><span data-stu-id="15606-142">String</span></span>|<span data-ttu-id="15606-143">PFX 証明書のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="15606-143">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="15606-144">startDateTime</span><span class="sxs-lookup"><span data-stu-id="15606-144">startDateTime</span></span>|<span data-ttu-id="15606-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15606-145">DateTimeOffset</span></span>|<span data-ttu-id="15606-146">証明書の有効性は、日付と時刻を開始します。</span><span class="sxs-lookup"><span data-stu-id="15606-146">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="15606-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="15606-147">expirationDateTime</span></span>|<span data-ttu-id="15606-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15606-148">DateTimeOffset</span></span>|<span data-ttu-id="15606-149">証明書の有効期限切れ日時です。</span><span class="sxs-lookup"><span data-stu-id="15606-149">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="15606-150">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="15606-150">providerName</span></span>|<span data-ttu-id="15606-151">String</span><span class="sxs-lookup"><span data-stu-id="15606-151">String</span></span>|<span data-ttu-id="15606-152">暗号サービス プロバイダーがこの blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="15606-152">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="15606-153">キー名</span><span class="sxs-lookup"><span data-stu-id="15606-153">keyName</span></span>|<span data-ttu-id="15606-154">String</span><span class="sxs-lookup"><span data-stu-id="15606-154">String</span></span>|<span data-ttu-id="15606-155">(プロバイダー) 内のキーの名前が blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="15606-155">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="15606-156">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="15606-156">paddingScheme</span></span>|[<span data-ttu-id="15606-157">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="15606-157">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="15606-158">暗号化/復号化中に、プロバイダーによって使用されるスキームをパディングします。</span><span class="sxs-lookup"><span data-stu-id="15606-158">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="15606-159">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="15606-159">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="15606-160">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="15606-160">encryptedPfxBlob</span></span>|<span data-ttu-id="15606-161">Binary</span><span class="sxs-lookup"><span data-stu-id="15606-161">Binary</span></span>|<span data-ttu-id="15606-162">PFX の暗号化された blob です。</span><span class="sxs-lookup"><span data-stu-id="15606-162">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="15606-163">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="15606-163">encryptedPfxPassword</span></span>|<span data-ttu-id="15606-164">String</span><span class="sxs-lookup"><span data-stu-id="15606-164">String</span></span>|<span data-ttu-id="15606-165">PFX パスワードを暗号化します。</span><span class="sxs-lookup"><span data-stu-id="15606-165">Encrypted PFX password.</span></span>|
|<span data-ttu-id="15606-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15606-166">createdDateTime</span></span>|<span data-ttu-id="15606-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15606-167">DateTimeOffset</span></span>|<span data-ttu-id="15606-168">PFX 証明書がインポートされたときに、日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="15606-168">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="15606-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15606-169">lastModifiedDateTime</span></span>|<span data-ttu-id="15606-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15606-170">DateTimeOffset</span></span>|<span data-ttu-id="15606-171">PFX 証明書が最後に修正された日時です。</span><span class="sxs-lookup"><span data-stu-id="15606-171">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15606-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15606-172">Relationships</span></span>
<span data-ttu-id="15606-173">なし</span><span class="sxs-lookup"><span data-stu-id="15606-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15606-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15606-174">JSON Representation</span></span>
<span data-ttu-id="15606-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15606-175">Here is a JSON representation of the resource.</span></span>
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




