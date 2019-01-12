---
title: デバイスを更新する
description: デバイスのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42471e32eac050b84e36477c1cd48fd06feb4244
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916377"
---
# <a name="update-device"></a><span data-ttu-id="08d38-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="08d38-103">Update device</span></span>

> <span data-ttu-id="08d38-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08d38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08d38-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08d38-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08d38-106">デバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="08d38-106">Update the properties of a device.</span></span>

<span data-ttu-id="08d38-107">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="08d38-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="08d38-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08d38-108">Permissions</span></span>
<span data-ttu-id="08d38-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08d38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08d38-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08d38-111">Permission type</span></span>      | <span data-ttu-id="08d38-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08d38-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08d38-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08d38-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08d38-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08d38-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="08d38-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08d38-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08d38-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08d38-116">Not supported.</span></span> |
|<span data-ttu-id="08d38-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08d38-117">Application</span></span> | <span data-ttu-id="08d38-118">非サポート</span><span class="sxs-lookup"><span data-stu-id="08d38-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="08d38-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08d38-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="08d38-120">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="08d38-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08d38-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08d38-121">Request headers</span></span>
| <span data-ttu-id="08d38-122">名前</span><span class="sxs-lookup"><span data-stu-id="08d38-122">Name</span></span>       | <span data-ttu-id="08d38-123">型</span><span class="sxs-lookup"><span data-stu-id="08d38-123">Type</span></span> | <span data-ttu-id="08d38-124">説明</span><span class="sxs-lookup"><span data-stu-id="08d38-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="08d38-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08d38-125">Authorization</span></span>  | <span data-ttu-id="08d38-126">string</span><span class="sxs-lookup"><span data-stu-id="08d38-126">string</span></span>  | <span data-ttu-id="08d38-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08d38-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08d38-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="08d38-129">Request body</span></span>

<span data-ttu-id="08d38-130">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="08d38-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="08d38-131">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="08d38-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="08d38-132">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="08d38-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08d38-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08d38-133">Property</span></span>     | <span data-ttu-id="08d38-134">型</span><span class="sxs-lookup"><span data-stu-id="08d38-134">Type</span></span>   |<span data-ttu-id="08d38-135">説明</span><span class="sxs-lookup"><span data-stu-id="08d38-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08d38-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="08d38-136">accountEnabled</span></span>|<span data-ttu-id="08d38-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="08d38-137">Boolean</span></span>| <span data-ttu-id="08d38-138">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="08d38-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="08d38-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="08d38-139">operatingSystem</span></span>|<span data-ttu-id="08d38-140">文字列</span><span class="sxs-lookup"><span data-stu-id="08d38-140">String</span></span>|<span data-ttu-id="08d38-141">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="08d38-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="08d38-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="08d38-142">operatingSystemVersion</span></span>|<span data-ttu-id="08d38-143">String</span><span class="sxs-lookup"><span data-stu-id="08d38-143">String</span></span>|<span data-ttu-id="08d38-144">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="08d38-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="08d38-145">displayName</span><span class="sxs-lookup"><span data-stu-id="08d38-145">displayName</span></span>|<span data-ttu-id="08d38-146">文字列</span><span class="sxs-lookup"><span data-stu-id="08d38-146">String</span></span>|<span data-ttu-id="08d38-147">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="08d38-147">The display name for the device.</span></span>|
|<span data-ttu-id="08d38-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="08d38-148">isCompliant</span></span>|<span data-ttu-id="08d38-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d38-149">Boolean</span></span>|<span data-ttu-id="08d38-150">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="08d38-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="08d38-151">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="08d38-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="08d38-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="08d38-152">isManaged</span></span>|<span data-ttu-id="08d38-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d38-153">Boolean</span></span>|<span data-ttu-id="08d38-154">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="08d38-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="08d38-155">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="08d38-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="08d38-156">使用することができます、**デバイス**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**デバイス**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="08d38-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="08d38-157">応答</span><span class="sxs-lookup"><span data-stu-id="08d38-157">Response</span></span>

<span data-ttu-id="08d38-158">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="08d38-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08d38-159">例</span><span class="sxs-lookup"><span data-stu-id="08d38-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08d38-160">要求</span><span class="sxs-lookup"><span data-stu-id="08d38-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="08d38-161">応答</span><span class="sxs-lookup"><span data-stu-id="08d38-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="08d38-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="08d38-162">See also</span></span>

- [<span data-ttu-id="08d38-163">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="08d38-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="08d38-164">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="08d38-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="08d38-165">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="08d38-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
