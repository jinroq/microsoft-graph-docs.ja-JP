---
title: デバイスを更新する
description: 登録済みデバイスのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f24372e122045eee9d79cde6334038f0dc1ccddf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583509"
---
# <a name="update-device"></a><span data-ttu-id="9abac-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="9abac-103">Update device</span></span>

<span data-ttu-id="9abac-104">登録済みデバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9abac-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="9abac-105">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="9abac-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="9abac-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9abac-106">Permissions</span></span>
<span data-ttu-id="9abac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9abac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9abac-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9abac-109">Permission type</span></span>      | <span data-ttu-id="9abac-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9abac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9abac-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9abac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9abac-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9abac-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9abac-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9abac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9abac-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9abac-114">Not supported.</span></span> |
|<span data-ttu-id="9abac-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9abac-115">Application</span></span> | <span data-ttu-id="9abac-116">非サポート</span><span class="sxs-lookup"><span data-stu-id="9abac-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="9abac-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9abac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="9abac-118">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="9abac-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9abac-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9abac-119">Request headers</span></span>
| <span data-ttu-id="9abac-120">名前</span><span class="sxs-lookup"><span data-stu-id="9abac-120">Name</span></span>       | <span data-ttu-id="9abac-121">型</span><span class="sxs-lookup"><span data-stu-id="9abac-121">Type</span></span> | <span data-ttu-id="9abac-122">説明</span><span class="sxs-lookup"><span data-stu-id="9abac-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9abac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9abac-123">Authorization</span></span>  | <span data-ttu-id="9abac-124">string</span><span class="sxs-lookup"><span data-stu-id="9abac-124">string</span></span>  | <span data-ttu-id="9abac-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9abac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9abac-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9abac-127">Request body</span></span>

<span data-ttu-id="9abac-128">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9abac-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="9abac-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="9abac-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9abac-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9abac-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9abac-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9abac-131">Property</span></span>     | <span data-ttu-id="9abac-132">型</span><span class="sxs-lookup"><span data-stu-id="9abac-132">Type</span></span>   |<span data-ttu-id="9abac-133">説明</span><span class="sxs-lookup"><span data-stu-id="9abac-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9abac-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="9abac-134">accountEnabled</span></span>|<span data-ttu-id="9abac-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="9abac-135">Boolean</span></span>| <span data-ttu-id="9abac-136">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="9abac-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="9abac-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9abac-137">operatingSystem</span></span>|<span data-ttu-id="9abac-138">文字列</span><span class="sxs-lookup"><span data-stu-id="9abac-138">String</span></span>|<span data-ttu-id="9abac-139">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="9abac-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="9abac-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="9abac-140">operatingSystemVersion</span></span>|<span data-ttu-id="9abac-141">String</span><span class="sxs-lookup"><span data-stu-id="9abac-141">String</span></span>|<span data-ttu-id="9abac-142">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="9abac-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="9abac-143">displayName</span><span class="sxs-lookup"><span data-stu-id="9abac-143">displayName</span></span>|<span data-ttu-id="9abac-144">String</span><span class="sxs-lookup"><span data-stu-id="9abac-144">String</span></span>|<span data-ttu-id="9abac-145">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="9abac-145">The display name for the device.</span></span>|
|<span data-ttu-id="9abac-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="9abac-146">isCompliant</span></span>|<span data-ttu-id="9abac-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="9abac-147">Boolean</span></span>|<span data-ttu-id="9abac-148">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="9abac-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="9abac-149">これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。</span><span class="sxs-lookup"><span data-stu-id="9abac-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="9abac-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="9abac-150">isManaged</span></span>|<span data-ttu-id="9abac-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="9abac-151">Boolean</span></span>|<span data-ttu-id="9abac-152">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="9abac-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="9abac-153">これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。</span><span class="sxs-lookup"><span data-stu-id="9abac-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="9abac-154">応答</span><span class="sxs-lookup"><span data-stu-id="9abac-154">Response</span></span>

<span data-ttu-id="9abac-155">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9abac-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9abac-156">例</span><span class="sxs-lookup"><span data-stu-id="9abac-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9abac-157">要求</span><span class="sxs-lookup"><span data-stu-id="9abac-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="9abac-158">応答</span><span class="sxs-lookup"><span data-stu-id="9abac-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
