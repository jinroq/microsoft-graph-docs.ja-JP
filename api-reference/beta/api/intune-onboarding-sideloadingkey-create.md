---
title: SideLoadingKey を作成する
description: 新しい sideLoadingKey オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9bbd650c8c82f861d7e133447d7687d78ba86a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993999"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="81c5a-103">SideLoadingKey を作成する</span><span class="sxs-lookup"><span data-stu-id="81c5a-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="81c5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81c5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81c5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81c5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81c5a-106">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="81c5a-106">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81c5a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="81c5a-107">Prerequisites</span></span>
<span data-ttu-id="81c5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81c5a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81c5a-110">Permission type</span></span>|<span data-ttu-id="81c5a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81c5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81c5a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81c5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81c5a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81c5a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81c5a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81c5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81c5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81c5a-115">Not supported.</span></span>|
|<span data-ttu-id="81c5a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81c5a-116">Application</span></span>|<span data-ttu-id="81c5a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81c5a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81c5a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81c5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="81c5a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81c5a-119">Request headers</span></span>
|<span data-ttu-id="81c5a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81c5a-120">Header</span></span>|<span data-ttu-id="81c5a-121">値</span><span class="sxs-lookup"><span data-stu-id="81c5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81c5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81c5a-122">Authorization</span></span>|<span data-ttu-id="81c5a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="81c5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81c5a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="81c5a-124">Accept</span></span>|<span data-ttu-id="81c5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81c5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81c5a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="81c5a-126">Request body</span></span>
<span data-ttu-id="81c5a-127">要求本文で、sideLoadingKey オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81c5a-127">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="81c5a-128">次の表に、sideLoadingKey の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="81c5a-128">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="81c5a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81c5a-129">Property</span></span>|<span data-ttu-id="81c5a-130">型</span><span class="sxs-lookup"><span data-stu-id="81c5a-130">Type</span></span>|<span data-ttu-id="81c5a-131">説明</span><span class="sxs-lookup"><span data-stu-id="81c5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81c5a-132">id</span><span class="sxs-lookup"><span data-stu-id="81c5a-132">id</span></span>|<span data-ttu-id="81c5a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="81c5a-133">String</span></span>|<span data-ttu-id="81c5a-134">サイドローディングキーの一意 Id。</span><span class="sxs-lookup"><span data-stu-id="81c5a-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="81c5a-135">value</span><span class="sxs-lookup"><span data-stu-id="81c5a-135">value</span></span>|<span data-ttu-id="81c5a-136">文字列</span><span class="sxs-lookup"><span data-stu-id="81c5a-136">String</span></span>|<span data-ttu-id="81c5a-137">サイドローディングキー値は、5 x 5 の値で、hiphens で区切られています。</span><span class="sxs-lookup"><span data-stu-id="81c5a-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="81c5a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="81c5a-138">displayName</span></span>|<span data-ttu-id="81c5a-139">String</span><span class="sxs-lookup"><span data-stu-id="81c5a-139">String</span></span>|<span data-ttu-id="81c5a-140">ITPro 管理者に表示されるサイドローディングキー名。</span><span class="sxs-lookup"><span data-stu-id="81c5a-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="81c5a-141">description</span><span class="sxs-lookup"><span data-stu-id="81c5a-141">description</span></span>|<span data-ttu-id="81c5a-142">String</span><span class="sxs-lookup"><span data-stu-id="81c5a-142">String</span></span>|<span data-ttu-id="81c5a-143">ITPro 管理者に表示されるサイドローディングキーの説明。</span><span class="sxs-lookup"><span data-stu-id="81c5a-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="81c5a-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="81c5a-144">totalActivation</span></span>|<span data-ttu-id="81c5a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="81c5a-145">Int32</span></span>|<span data-ttu-id="81c5a-146">ITPro 管理者に表示されるサイドローディングキーの合計です。</span><span class="sxs-lookup"><span data-stu-id="81c5a-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="81c5a-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="81c5a-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="81c5a-148">String</span><span class="sxs-lookup"><span data-stu-id="81c5a-148">String</span></span>|<span data-ttu-id="81c5a-149">サイドローディングキー最終更新日が ITPro の管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="81c5a-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="81c5a-150">応答</span><span class="sxs-lookup"><span data-stu-id="81c5a-150">Response</span></span>
<span data-ttu-id="81c5a-151">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81c5a-151">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81c5a-152">例</span><span class="sxs-lookup"><span data-stu-id="81c5a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="81c5a-153">要求</span><span class="sxs-lookup"><span data-stu-id="81c5a-153">Request</span></span>
<span data-ttu-id="81c5a-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81c5a-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
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

### <a name="response"></a><span data-ttu-id="81c5a-155">応答</span><span class="sxs-lookup"><span data-stu-id="81c5a-155">Response</span></span>
<span data-ttu-id="81c5a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81c5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





