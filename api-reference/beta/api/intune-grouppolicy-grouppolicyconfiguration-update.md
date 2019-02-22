---
title: grouppolicyconfiguration を更新する
description: grouppolicyconfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 867d70f3978db683cb154b9e5405df08b315b4b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160033"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="a562f-103">grouppolicyconfiguration を更新する</span><span class="sxs-lookup"><span data-stu-id="a562f-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="a562f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a562f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a562f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a562f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a562f-106">[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a562f-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a562f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a562f-107">Prerequisites</span></span>
<span data-ttu-id="a562f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a562f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a562f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a562f-110">Permission type</span></span>|<span data-ttu-id="a562f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a562f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a562f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a562f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a562f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a562f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a562f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a562f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a562f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a562f-115">Not supported.</span></span>|
|<span data-ttu-id="a562f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a562f-116">Application</span></span>|<span data-ttu-id="a562f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a562f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a562f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a562f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a562f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a562f-119">Request headers</span></span>
|<span data-ttu-id="a562f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a562f-120">Header</span></span>|<span data-ttu-id="a562f-121">値</span><span class="sxs-lookup"><span data-stu-id="a562f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a562f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a562f-122">Authorization</span></span>|<span data-ttu-id="a562f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a562f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a562f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a562f-124">Accept</span></span>|<span data-ttu-id="a562f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a562f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a562f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a562f-126">Request body</span></span>
<span data-ttu-id="a562f-127">要求本文で、 [grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a562f-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="a562f-128">次の表に、 [grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a562f-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="a562f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a562f-129">Property</span></span>|<span data-ttu-id="a562f-130">型</span><span class="sxs-lookup"><span data-stu-id="a562f-130">Type</span></span>|<span data-ttu-id="a562f-131">説明</span><span class="sxs-lookup"><span data-stu-id="a562f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a562f-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a562f-132">createdDateTime</span></span>|<span data-ttu-id="a562f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a562f-133">DateTimeOffset</span></span>|<span data-ttu-id="a562f-134">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a562f-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="a562f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a562f-135">displayName</span></span>|<span data-ttu-id="a562f-136">String</span><span class="sxs-lookup"><span data-stu-id="a562f-136">String</span></span>|<span data-ttu-id="a562f-137">ユーザーが指定した resource オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="a562f-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="a562f-138">説明</span><span class="sxs-lookup"><span data-stu-id="a562f-138">description</span></span>|<span data-ttu-id="a562f-139">String</span><span class="sxs-lookup"><span data-stu-id="a562f-139">String</span></span>|<span data-ttu-id="a562f-140">ユーザーが指定した resource オブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="a562f-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="a562f-141">id</span><span class="sxs-lookup"><span data-stu-id="a562f-141">id</span></span>|<span data-ttu-id="a562f-142">String</span><span class="sxs-lookup"><span data-stu-id="a562f-142">String</span></span>|<span data-ttu-id="a562f-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a562f-143">Key of the entity.</span></span>|
|<span data-ttu-id="a562f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a562f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a562f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a562f-145">DateTimeOffset</span></span>|<span data-ttu-id="a562f-146">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a562f-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a562f-147">応答</span><span class="sxs-lookup"><span data-stu-id="a562f-147">Response</span></span>
<span data-ttu-id="a562f-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a562f-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a562f-149">例</span><span class="sxs-lookup"><span data-stu-id="a562f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a562f-150">要求</span><span class="sxs-lookup"><span data-stu-id="a562f-150">Request</span></span>
<span data-ttu-id="a562f-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a562f-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="a562f-152">応答</span><span class="sxs-lookup"><span data-stu-id="a562f-152">Response</span></span>
<span data-ttu-id="a562f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a562f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




