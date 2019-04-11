---
title: grouppolicyconfiguration の作成
description: 新しい grouppolicyconfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd0c63b1d8c8df449a68cbeb64f391adb659ae64
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805370"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="8b652-103">grouppolicyconfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="8b652-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="8b652-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b652-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b652-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b652-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b652-106">新しい[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8b652-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b652-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8b652-107">Prerequisites</span></span>
<span data-ttu-id="8b652-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b652-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b652-110">Permission type</span></span>|<span data-ttu-id="8b652-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b652-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b652-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b652-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b652-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b652-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b652-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b652-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b652-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b652-115">Not supported.</span></span>|
|<span data-ttu-id="8b652-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b652-116">Application</span></span>|<span data-ttu-id="8b652-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b652-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b652-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b652-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8b652-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b652-119">Request headers</span></span>
|<span data-ttu-id="8b652-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b652-120">Header</span></span>|<span data-ttu-id="8b652-121">値</span><span class="sxs-lookup"><span data-stu-id="8b652-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b652-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b652-122">Authorization</span></span>|<span data-ttu-id="8b652-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b652-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b652-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8b652-124">Accept</span></span>|<span data-ttu-id="8b652-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b652-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b652-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b652-126">Request body</span></span>
<span data-ttu-id="8b652-127">要求本文で、grouppolicyconfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8b652-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="8b652-128">次の表に、grouppolicyconfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8b652-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="8b652-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b652-129">Property</span></span>|<span data-ttu-id="8b652-130">型</span><span class="sxs-lookup"><span data-stu-id="8b652-130">Type</span></span>|<span data-ttu-id="8b652-131">説明</span><span class="sxs-lookup"><span data-stu-id="8b652-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b652-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b652-132">createdDateTime</span></span>|<span data-ttu-id="8b652-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b652-133">DateTimeOffset</span></span>|<span data-ttu-id="8b652-134">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8b652-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="8b652-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8b652-135">displayName</span></span>|<span data-ttu-id="8b652-136">String</span><span class="sxs-lookup"><span data-stu-id="8b652-136">String</span></span>|<span data-ttu-id="8b652-137">ユーザーが指定した resource オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="8b652-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="8b652-138">説明</span><span class="sxs-lookup"><span data-stu-id="8b652-138">description</span></span>|<span data-ttu-id="8b652-139">String</span><span class="sxs-lookup"><span data-stu-id="8b652-139">String</span></span>|<span data-ttu-id="8b652-140">ユーザーが指定した resource オブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="8b652-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="8b652-141">id</span><span class="sxs-lookup"><span data-stu-id="8b652-141">id</span></span>|<span data-ttu-id="8b652-142">String</span><span class="sxs-lookup"><span data-stu-id="8b652-142">String</span></span>|<span data-ttu-id="8b652-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8b652-143">Key of the entity.</span></span>|
|<span data-ttu-id="8b652-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b652-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8b652-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b652-145">DateTimeOffset</span></span>|<span data-ttu-id="8b652-146">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8b652-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8b652-147">応答</span><span class="sxs-lookup"><span data-stu-id="8b652-147">Response</span></span>
<span data-ttu-id="8b652-148">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8b652-148">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b652-149">例</span><span class="sxs-lookup"><span data-stu-id="8b652-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b652-150">要求</span><span class="sxs-lookup"><span data-stu-id="8b652-150">Request</span></span>
<span data-ttu-id="8b652-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b652-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="8b652-152">応答</span><span class="sxs-lookup"><span data-stu-id="8b652-152">Response</span></span>
<span data-ttu-id="8b652-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b652-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





