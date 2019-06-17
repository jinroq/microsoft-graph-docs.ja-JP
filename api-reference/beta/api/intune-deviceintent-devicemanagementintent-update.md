---
title: DeviceManagementIntent の更新
description: DeviceManagementIntent オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd8b85ccab0153b749ff29be13187e3fd2fd4ef6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960448"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="3c4c7-103">DeviceManagementIntent の更新</span><span class="sxs-lookup"><span data-stu-id="3c4c7-103">Update deviceManagementIntent</span></span>

> <span data-ttu-id="3c4c7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c4c7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c4c7-106">[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-106">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c4c7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c4c7-107">Prerequisites</span></span>
<span data-ttu-id="3c4c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c4c7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c4c7-110">Permission type</span></span>|<span data-ttu-id="3c4c7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c4c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c4c7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c4c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c4c7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c4c7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c4c7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c4c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c4c7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-115">Not supported.</span></span>|
|<span data-ttu-id="3c4c7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c4c7-116">Application</span></span>|<span data-ttu-id="3c4c7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c4c7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c4c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="3c4c7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c4c7-119">Request headers</span></span>
|<span data-ttu-id="3c4c7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c4c7-120">Header</span></span>|<span data-ttu-id="3c4c7-121">値</span><span class="sxs-lookup"><span data-stu-id="3c4c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c4c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c4c7-122">Authorization</span></span>|<span data-ttu-id="3c4c7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c4c7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3c4c7-124">Accept</span></span>|<span data-ttu-id="3c4c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c4c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c4c7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c4c7-126">Request body</span></span>
<span data-ttu-id="3c4c7-127">要求本文で、 [Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-127">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="3c4c7-128">次の表に、 [Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-128">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="3c4c7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c4c7-129">Property</span></span>|<span data-ttu-id="3c4c7-130">型</span><span class="sxs-lookup"><span data-stu-id="3c4c7-130">Type</span></span>|<span data-ttu-id="3c4c7-131">説明</span><span class="sxs-lookup"><span data-stu-id="3c4c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c4c7-132">id</span><span class="sxs-lookup"><span data-stu-id="3c4c7-132">id</span></span>|<span data-ttu-id="3c4c7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3c4c7-133">String</span></span>|<span data-ttu-id="3c4c7-134">インテント ID</span><span class="sxs-lookup"><span data-stu-id="3c4c7-134">The intent ID</span></span>|
|<span data-ttu-id="3c4c7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3c4c7-135">displayName</span></span>|<span data-ttu-id="3c4c7-136">String</span><span class="sxs-lookup"><span data-stu-id="3c4c7-136">String</span></span>|<span data-ttu-id="3c4c7-137">ユーザーが指定した表示名</span><span class="sxs-lookup"><span data-stu-id="3c4c7-137">The user given display name</span></span>|
|<span data-ttu-id="3c4c7-138">description</span><span class="sxs-lookup"><span data-stu-id="3c4c7-138">description</span></span>|<span data-ttu-id="3c4c7-139">String</span><span class="sxs-lookup"><span data-stu-id="3c4c7-139">String</span></span>|<span data-ttu-id="3c4c7-140">ユーザーが指定した説明</span><span class="sxs-lookup"><span data-stu-id="3c4c7-140">The user given description</span></span>|
|<span data-ttu-id="3c4c7-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3c4c7-141">isAssigned</span></span>|<span data-ttu-id="3c4c7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c4c7-142">Boolean</span></span>|<span data-ttu-id="3c4c7-143">目的がユーザーに割り当てられているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="3c4c7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c4c7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3c4c7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c4c7-145">DateTimeOffset</span></span>|<span data-ttu-id="3c4c7-146">目的が最後に変更された日時</span><span class="sxs-lookup"><span data-stu-id="3c4c7-146">When the intent was last modified</span></span>|
|<span data-ttu-id="3c4c7-147">templateId</span><span class="sxs-lookup"><span data-stu-id="3c4c7-147">templateId</span></span>|<span data-ttu-id="3c4c7-148">String</span><span class="sxs-lookup"><span data-stu-id="3c4c7-148">String</span></span>|<span data-ttu-id="3c4c7-149">この目的が作成されたテンプレートの ID (存在する場合)</span><span class="sxs-lookup"><span data-stu-id="3c4c7-149">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="3c4c7-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3c4c7-150">roleScopeTagIds</span></span>|<span data-ttu-id="3c4c7-151">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3c4c7-151">String collection</span></span>|<span data-ttu-id="3c4c7-152">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3c4c7-153">応答</span><span class="sxs-lookup"><span data-stu-id="3c4c7-153">Response</span></span>
<span data-ttu-id="3c4c7-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c4c7-155">例</span><span class="sxs-lookup"><span data-stu-id="3c4c7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c4c7-156">要求</span><span class="sxs-lookup"><span data-stu-id="3c4c7-156">Request</span></span>
<span data-ttu-id="3c4c7-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3c4c7-158">応答</span><span class="sxs-lookup"><span data-stu-id="3c4c7-158">Response</span></span>
<span data-ttu-id="3c4c7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c4c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





