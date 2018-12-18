---
title: デバイスを更新する
description: デバイスのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: df86581c1edb531e822204698486358fac29f106
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356561"
---
# <a name="update-device"></a><span data-ttu-id="956f4-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="956f4-103">Update device</span></span>

> <span data-ttu-id="956f4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="956f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="956f4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="956f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="956f4-106">デバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="956f4-106">Update the properties of a device.</span></span>

<span data-ttu-id="956f4-107">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="956f4-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="956f4-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="956f4-108">Permissions</span></span>
<span data-ttu-id="956f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="956f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956f4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="956f4-111">Permission type</span></span>      | <span data-ttu-id="956f4-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="956f4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="956f4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="956f4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="956f4-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="956f4-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="956f4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="956f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="956f4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="956f4-116">Not supported.</span></span> |
|<span data-ttu-id="956f4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="956f4-117">Application</span></span> | <span data-ttu-id="956f4-118">非サポート</span><span class="sxs-lookup"><span data-stu-id="956f4-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="956f4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="956f4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="956f4-120">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="956f4-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="956f4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="956f4-121">Request headers</span></span>
| <span data-ttu-id="956f4-122">名前</span><span class="sxs-lookup"><span data-stu-id="956f4-122">Name</span></span>       | <span data-ttu-id="956f4-123">種類</span><span class="sxs-lookup"><span data-stu-id="956f4-123">Type</span></span> | <span data-ttu-id="956f4-124">説明</span><span class="sxs-lookup"><span data-stu-id="956f4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="956f4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="956f4-125">Authorization</span></span>  | <span data-ttu-id="956f4-126">string</span><span class="sxs-lookup"><span data-stu-id="956f4-126">string</span></span>  | <span data-ttu-id="956f4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="956f4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="956f4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="956f4-129">Request body</span></span>

<span data-ttu-id="956f4-130">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="956f4-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="956f4-131">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="956f4-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="956f4-132">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="956f4-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="956f4-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="956f4-133">Property</span></span>     | <span data-ttu-id="956f4-134">種類</span><span class="sxs-lookup"><span data-stu-id="956f4-134">Type</span></span>   |<span data-ttu-id="956f4-135">説明</span><span class="sxs-lookup"><span data-stu-id="956f4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="956f4-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="956f4-136">accountEnabled</span></span>|<span data-ttu-id="956f4-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="956f4-137">Boolean</span></span>| <span data-ttu-id="956f4-138">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="956f4-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="956f4-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="956f4-139">operatingSystem</span></span>|<span data-ttu-id="956f4-140">文字列</span><span class="sxs-lookup"><span data-stu-id="956f4-140">String</span></span>|<span data-ttu-id="956f4-141">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="956f4-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="956f4-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="956f4-142">operatingSystemVersion</span></span>|<span data-ttu-id="956f4-143">String</span><span class="sxs-lookup"><span data-stu-id="956f4-143">String</span></span>|<span data-ttu-id="956f4-144">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="956f4-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="956f4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="956f4-145">displayName</span></span>|<span data-ttu-id="956f4-146">文字列</span><span class="sxs-lookup"><span data-stu-id="956f4-146">String</span></span>|<span data-ttu-id="956f4-147">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="956f4-147">The display name for the device.</span></span>|
|<span data-ttu-id="956f4-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="956f4-148">isCompliant</span></span>|<span data-ttu-id="956f4-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="956f4-149">Boolean</span></span>|<span data-ttu-id="956f4-150">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="956f4-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="956f4-151">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="956f4-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="956f4-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="956f4-152">isManaged</span></span>|<span data-ttu-id="956f4-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="956f4-153">Boolean</span></span>|<span data-ttu-id="956f4-154">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="956f4-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="956f4-155">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="956f4-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="956f4-156">使用することができます、**デバイス**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**デバイス**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="956f4-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="956f4-157">応答</span><span class="sxs-lookup"><span data-stu-id="956f4-157">Response</span></span>

<span data-ttu-id="956f4-158">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="956f4-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="956f4-159">例</span><span class="sxs-lookup"><span data-stu-id="956f4-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="956f4-160">要求</span><span class="sxs-lookup"><span data-stu-id="956f4-160">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="956f4-161">応答</span><span class="sxs-lookup"><span data-stu-id="956f4-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="956f4-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="956f4-162">See also</span></span>

- [<span data-ttu-id="956f4-163">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="956f4-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="956f4-164">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="956f4-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="956f4-165">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="956f4-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
