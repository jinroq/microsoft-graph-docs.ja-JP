---
title: デバイスを更新する
description: 登録済みデバイスのプロパティを更新します。
ms.openlocfilehash: cb2f23a5c36b22b65503ea0e8ac93af443c13e08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021269"
---
# <a name="update-device"></a><span data-ttu-id="8e4d5-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="8e4d5-103">Update device</span></span>

<span data-ttu-id="8e4d5-104">登録済みデバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="8e4d5-105">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e4d5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e4d5-106">Permissions</span></span>
<span data-ttu-id="8e4d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e4d5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e4d5-109">Permission type</span></span>      | <span data-ttu-id="8e4d5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e4d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e4d5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e4d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e4d5-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e4d5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8e4d5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e4d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e4d5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-114">Not supported.</span></span> |
|<span data-ttu-id="8e4d5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e4d5-115">Application</span></span> | <span data-ttu-id="8e4d5-116">非サポート</span><span class="sxs-lookup"><span data-stu-id="8e4d5-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e4d5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e4d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="8e4d5-118">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e4d5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e4d5-119">Request headers</span></span>
| <span data-ttu-id="8e4d5-120">名前</span><span class="sxs-lookup"><span data-stu-id="8e4d5-120">Name</span></span>       | <span data-ttu-id="8e4d5-121">型</span><span class="sxs-lookup"><span data-stu-id="8e4d5-121">Type</span></span> | <span data-ttu-id="8e4d5-122">説明</span><span class="sxs-lookup"><span data-stu-id="8e4d5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e4d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e4d5-123">Authorization</span></span>  | <span data-ttu-id="8e4d5-124">string</span><span class="sxs-lookup"><span data-stu-id="8e4d5-124">string</span></span>  | <span data-ttu-id="8e4d5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e4d5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e4d5-127">Request body</span></span>

<span data-ttu-id="8e4d5-128">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="8e4d5-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8e4d5-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e4d5-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e4d5-131">Property</span></span>     | <span data-ttu-id="8e4d5-132">型</span><span class="sxs-lookup"><span data-stu-id="8e4d5-132">Type</span></span>   |<span data-ttu-id="8e4d5-133">説明</span><span class="sxs-lookup"><span data-stu-id="8e4d5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e4d5-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="8e4d5-134">accountEnabled</span></span>|<span data-ttu-id="8e4d5-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="8e4d5-135">Boolean</span></span>| <span data-ttu-id="8e4d5-136">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="8e4d5-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e4d5-137">operatingSystem</span></span>|<span data-ttu-id="8e4d5-138">文字列</span><span class="sxs-lookup"><span data-stu-id="8e4d5-138">String</span></span>|<span data-ttu-id="8e4d5-139">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="8e4d5-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="8e4d5-140">operatingSystemVersion</span></span>|<span data-ttu-id="8e4d5-141">String</span><span class="sxs-lookup"><span data-stu-id="8e4d5-141">String</span></span>|<span data-ttu-id="8e4d5-142">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="8e4d5-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="8e4d5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8e4d5-143">displayName</span></span>|<span data-ttu-id="8e4d5-144">文字列</span><span class="sxs-lookup"><span data-stu-id="8e4d5-144">String</span></span>|<span data-ttu-id="8e4d5-145">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-145">The display name for the device.</span></span>|
|<span data-ttu-id="8e4d5-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="8e4d5-146">isCompliant</span></span>|<span data-ttu-id="8e4d5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e4d5-147">Boolean</span></span>|<span data-ttu-id="8e4d5-148">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="8e4d5-149">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="8e4d5-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="8e4d5-150">isManaged</span></span>|<span data-ttu-id="8e4d5-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e4d5-151">Boolean</span></span>|<span data-ttu-id="8e4d5-152">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="8e4d5-153">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="8e4d5-154">応答</span><span class="sxs-lookup"><span data-stu-id="8e4d5-154">Response</span></span>

<span data-ttu-id="8e4d5-155">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8e4d5-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e4d5-156">例</span><span class="sxs-lookup"><span data-stu-id="8e4d5-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e4d5-157">要求</span><span class="sxs-lookup"><span data-stu-id="8e4d5-157">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="8e4d5-158">応答</span><span class="sxs-lookup"><span data-stu-id="8e4d5-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
