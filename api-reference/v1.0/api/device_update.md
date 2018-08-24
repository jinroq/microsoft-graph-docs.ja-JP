# <a name="update-device"></a><span data-ttu-id="b8c7c-101">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="b8c7c-101">Update device</span></span>

<span data-ttu-id="b8c7c-102">登録済みデバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-102">Update the properties of a registered device.</span></span>

<span data-ttu-id="b8c7c-103">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-103">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c7c-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8c7c-104">Permissions</span></span>
<span data-ttu-id="b8c7c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8c7c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8c7c-107">Permission type</span></span>      | <span data-ttu-id="b8c7c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8c7c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8c7c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8c7c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b8c7c-110">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8c7c-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b8c7c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8c7c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8c7c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-112">Not supported.</span></span> |
|<span data-ttu-id="b8c7c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8c7c-113">Application</span></span> | <span data-ttu-id="b8c7c-114">非サポート</span><span class="sxs-lookup"><span data-stu-id="b8c7c-114">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8c7c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8c7c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="b8c7c-116">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-116">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8c7c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8c7c-117">Request headers</span></span>
| <span data-ttu-id="b8c7c-118">名前</span><span class="sxs-lookup"><span data-stu-id="b8c7c-118">Name</span></span>       | <span data-ttu-id="b8c7c-119">型</span><span class="sxs-lookup"><span data-stu-id="b8c7c-119">Type</span></span> | <span data-ttu-id="b8c7c-120">説明</span><span class="sxs-lookup"><span data-stu-id="b8c7c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8c7c-121">承認</span><span class="sxs-lookup"><span data-stu-id="b8c7c-121">Authorization</span></span>  | <span data-ttu-id="b8c7c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="b8c7c-122">string</span></span>  | <span data-ttu-id="b8c7c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8c7c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8c7c-125">Request body</span></span>

<span data-ttu-id="b8c7c-126">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-126">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="b8c7c-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8c7c-128">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8c7c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8c7c-129">Property</span></span>     | <span data-ttu-id="b8c7c-130">型</span><span class="sxs-lookup"><span data-stu-id="b8c7c-130">Type</span></span>   |<span data-ttu-id="b8c7c-131">説明</span><span class="sxs-lookup"><span data-stu-id="b8c7c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8c7c-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b8c7c-132">accountEnabled</span></span>|<span data-ttu-id="b8c7c-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="b8c7c-133">Boolean</span></span>| <span data-ttu-id="b8c7c-134">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-134">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="b8c7c-135">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8c7c-135">operatingSystem</span></span>|<span data-ttu-id="b8c7c-136">文字列</span><span class="sxs-lookup"><span data-stu-id="b8c7c-136">String</span></span>|<span data-ttu-id="b8c7c-137">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-137">The type of operating system on the device.</span></span>|
|<span data-ttu-id="b8c7c-138">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="b8c7c-138">operatingSystemVersion</span></span>|<span data-ttu-id="b8c7c-139">文字列</span><span class="sxs-lookup"><span data-stu-id="b8c7c-139">String</span></span>|<span data-ttu-id="b8c7c-140">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="b8c7c-140">The version of the operating system on the device</span></span>|
|<span data-ttu-id="b8c7c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b8c7c-141">displayName</span></span>|<span data-ttu-id="b8c7c-142">文字列</span><span class="sxs-lookup"><span data-stu-id="b8c7c-142">String</span></span>|<span data-ttu-id="b8c7c-143">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-143">The display name for the device.</span></span>|
|<span data-ttu-id="b8c7c-144">isCompliant</span><span class="sxs-lookup"><span data-stu-id="b8c7c-144">isCompliant</span></span>|<span data-ttu-id="b8c7c-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="b8c7c-145">Boolean</span></span>|<span data-ttu-id="b8c7c-146">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-146">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="b8c7c-147">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-147">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="b8c7c-148">isManaged</span><span class="sxs-lookup"><span data-stu-id="b8c7c-148">isManaged</span></span>|<span data-ttu-id="b8c7c-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="b8c7c-149">Boolean</span></span>|<span data-ttu-id="b8c7c-150">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-150">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="b8c7c-151">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="b8c7c-152">応答</span><span class="sxs-lookup"><span data-stu-id="b8c7c-152">Response</span></span>

<span data-ttu-id="b8c7c-153">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b8c7c-153">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8c7c-154">例</span><span class="sxs-lookup"><span data-stu-id="b8c7c-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8c7c-155">要求</span><span class="sxs-lookup"><span data-stu-id="b8c7c-155">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="b8c7c-156">応答</span><span class="sxs-lookup"><span data-stu-id="b8c7c-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
