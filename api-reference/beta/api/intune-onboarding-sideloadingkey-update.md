---
title: SideLoadingKey の更新
description: SideLoadingKey オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4eaab991ffe7478dbe4485d9859c0f2f53cfad4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352386"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="ca4c0-103">SideLoadingKey の更新</span><span class="sxs-lookup"><span data-stu-id="ca4c0-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="ca4c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca4c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca4c0-106">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-106">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca4c0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca4c0-107">Prerequisites</span></span>
<span data-ttu-id="ca4c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca4c0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca4c0-110">Permission type</span></span>|<span data-ttu-id="ca4c0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca4c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca4c0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca4c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca4c0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca4c0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ca4c0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca4c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca4c0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-115">Not supported.</span></span>|
|<span data-ttu-id="ca4c0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca4c0-116">Application</span></span>|<span data-ttu-id="ca4c0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca4c0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca4c0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca4c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="ca4c0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca4c0-119">Request headers</span></span>
|<span data-ttu-id="ca4c0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca4c0-120">Header</span></span>|<span data-ttu-id="ca4c0-121">値</span><span class="sxs-lookup"><span data-stu-id="ca4c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca4c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca4c0-122">Authorization</span></span>|<span data-ttu-id="ca4c0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca4c0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ca4c0-124">Accept</span></span>|<span data-ttu-id="ca4c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca4c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca4c0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca4c0-126">Request body</span></span>
<span data-ttu-id="ca4c0-127">要求本文で、 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-127">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="ca4c0-128">次の表に、 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-128">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="ca4c0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca4c0-129">Property</span></span>|<span data-ttu-id="ca4c0-130">型</span><span class="sxs-lookup"><span data-stu-id="ca4c0-130">Type</span></span>|<span data-ttu-id="ca4c0-131">説明</span><span class="sxs-lookup"><span data-stu-id="ca4c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca4c0-132">id</span><span class="sxs-lookup"><span data-stu-id="ca4c0-132">id</span></span>|<span data-ttu-id="ca4c0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ca4c0-133">String</span></span>|<span data-ttu-id="ca4c0-134">サイドローディングキーの一意 Id。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="ca4c0-135">value</span><span class="sxs-lookup"><span data-stu-id="ca4c0-135">value</span></span>|<span data-ttu-id="ca4c0-136">文字列</span><span class="sxs-lookup"><span data-stu-id="ca4c0-136">String</span></span>|<span data-ttu-id="ca4c0-137">サイドローディングキー値は、5 x 5 の値で、hiphens で区切られています。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="ca4c0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ca4c0-138">displayName</span></span>|<span data-ttu-id="ca4c0-139">String</span><span class="sxs-lookup"><span data-stu-id="ca4c0-139">String</span></span>|<span data-ttu-id="ca4c0-140">ITPro 管理者に表示されるサイドローディングキー名。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ca4c0-141">description</span><span class="sxs-lookup"><span data-stu-id="ca4c0-141">description</span></span>|<span data-ttu-id="ca4c0-142">String</span><span class="sxs-lookup"><span data-stu-id="ca4c0-142">String</span></span>|<span data-ttu-id="ca4c0-143">ITPro 管理者に表示されるサイドローディングキーの説明。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="ca4c0-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="ca4c0-144">totalActivation</span></span>|<span data-ttu-id="ca4c0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ca4c0-145">Int32</span></span>|<span data-ttu-id="ca4c0-146">ITPro 管理者に表示されるサイドローディングキーの合計です。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ca4c0-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4c0-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="ca4c0-148">String</span><span class="sxs-lookup"><span data-stu-id="ca4c0-148">String</span></span>|<span data-ttu-id="ca4c0-149">サイドローディングキー最終更新日が ITPro の管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="ca4c0-150">応答</span><span class="sxs-lookup"><span data-stu-id="ca4c0-150">Response</span></span>
<span data-ttu-id="ca4c0-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-151">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca4c0-152">例</span><span class="sxs-lookup"><span data-stu-id="ca4c0-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca4c0-153">要求</span><span class="sxs-lookup"><span data-stu-id="ca4c0-153">Request</span></span>
<span data-ttu-id="ca4c0-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="ca4c0-155">応答</span><span class="sxs-lookup"><span data-stu-id="ca4c0-155">Response</span></span>
<span data-ttu-id="ca4c0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca4c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```






