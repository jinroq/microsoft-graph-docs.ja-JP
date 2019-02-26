---
title: groupPolicyPresentationValueLongDecimal の更新
description: groupPolicyPresentationValueLongDecimal オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b59ddc52cae02c762a85d7a93e317eab3f4f3df
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152277"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="40598-103">groupPolicyPresentationValueLongDecimal の更新</span><span class="sxs-lookup"><span data-stu-id="40598-103">Update groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="40598-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40598-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40598-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40598-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40598-106">[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40598-106">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40598-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="40598-107">Prerequisites</span></span>
<span data-ttu-id="40598-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40598-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40598-110">Permission type</span></span>|<span data-ttu-id="40598-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40598-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40598-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40598-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40598-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40598-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="40598-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40598-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40598-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40598-115">Not supported.</span></span>|
|<span data-ttu-id="40598-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40598-116">Application</span></span>|<span data-ttu-id="40598-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40598-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40598-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40598-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="40598-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40598-119">Request headers</span></span>
|<span data-ttu-id="40598-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40598-120">Header</span></span>|<span data-ttu-id="40598-121">値</span><span class="sxs-lookup"><span data-stu-id="40598-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40598-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40598-122">Authorization</span></span>|<span data-ttu-id="40598-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="40598-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40598-124">承諾</span><span class="sxs-lookup"><span data-stu-id="40598-124">Accept</span></span>|<span data-ttu-id="40598-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40598-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40598-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40598-126">Request body</span></span>
<span data-ttu-id="40598-127">要求本文で、 [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40598-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="40598-128">次の表に、 [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="40598-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="40598-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40598-129">Property</span></span>|<span data-ttu-id="40598-130">型</span><span class="sxs-lookup"><span data-stu-id="40598-130">Type</span></span>|<span data-ttu-id="40598-131">説明</span><span class="sxs-lookup"><span data-stu-id="40598-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40598-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40598-132">lastModifiedDateTime</span></span>|<span data-ttu-id="40598-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40598-133">DateTimeOffset</span></span>|<span data-ttu-id="40598-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="40598-134">The date and time the object was last modified.</span></span> <span data-ttu-id="40598-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40598-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="40598-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40598-136">createdDateTime</span></span>|<span data-ttu-id="40598-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40598-137">DateTimeOffset</span></span>|<span data-ttu-id="40598-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="40598-138">The date and time the object was created.</span></span> <span data-ttu-id="40598-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40598-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="40598-140">id</span><span class="sxs-lookup"><span data-stu-id="40598-140">id</span></span>|<span data-ttu-id="40598-141">String</span><span class="sxs-lookup"><span data-stu-id="40598-141">String</span></span>|<span data-ttu-id="40598-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="40598-142">Key of the entity.</span></span> <span data-ttu-id="40598-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="40598-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="40598-144">value</span><span class="sxs-lookup"><span data-stu-id="40598-144">value</span></span>|<span data-ttu-id="40598-145">Int64</span><span class="sxs-lookup"><span data-stu-id="40598-145">Int64</span></span>|<span data-ttu-id="40598-146">関連付けられたプレゼンテーションの符号なしの長整数型 (long) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="40598-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="40598-147">応答</span><span class="sxs-lookup"><span data-stu-id="40598-147">Response</span></span>
<span data-ttu-id="40598-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40598-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40598-149">例</span><span class="sxs-lookup"><span data-stu-id="40598-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="40598-150">要求</span><span class="sxs-lookup"><span data-stu-id="40598-150">Request</span></span>
<span data-ttu-id="40598-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40598-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="40598-152">応答</span><span class="sxs-lookup"><span data-stu-id="40598-152">Response</span></span>
<span data-ttu-id="40598-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40598-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




