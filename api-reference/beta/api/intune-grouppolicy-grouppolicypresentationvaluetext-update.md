---
title: groupPolicyPresentationValueText の更新
description: groupPolicyPresentationValueText オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59705a0463cd313cbc8fb8af0f267a09f5929fac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150933"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="457bb-103">groupPolicyPresentationValueText の更新</span><span class="sxs-lookup"><span data-stu-id="457bb-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="457bb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="457bb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="457bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="457bb-106">[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="457bb-106">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="457bb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="457bb-107">Prerequisites</span></span>
<span data-ttu-id="457bb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="457bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="457bb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="457bb-110">Permission type</span></span>|<span data-ttu-id="457bb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="457bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457bb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="457bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="457bb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457bb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="457bb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="457bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457bb-115">Not supported.</span></span>|
|<span data-ttu-id="457bb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="457bb-116">Application</span></span>|<span data-ttu-id="457bb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="457bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="457bb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="457bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="457bb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="457bb-119">Request headers</span></span>
|<span data-ttu-id="457bb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="457bb-120">Header</span></span>|<span data-ttu-id="457bb-121">値</span><span class="sxs-lookup"><span data-stu-id="457bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="457bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="457bb-122">Authorization</span></span>|<span data-ttu-id="457bb-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="457bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="457bb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="457bb-124">Accept</span></span>|<span data-ttu-id="457bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="457bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="457bb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="457bb-126">Request body</span></span>
<span data-ttu-id="457bb-127">要求本文で、 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="457bb-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="457bb-128">次の表に、 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="457bb-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="457bb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="457bb-129">Property</span></span>|<span data-ttu-id="457bb-130">型</span><span class="sxs-lookup"><span data-stu-id="457bb-130">Type</span></span>|<span data-ttu-id="457bb-131">説明</span><span class="sxs-lookup"><span data-stu-id="457bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457bb-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="457bb-132">lastModifiedDateTime</span></span>|<span data-ttu-id="457bb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457bb-133">DateTimeOffset</span></span>|<span data-ttu-id="457bb-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="457bb-134">The date and time the object was last modified.</span></span> <span data-ttu-id="457bb-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="457bb-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="457bb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="457bb-136">createdDateTime</span></span>|<span data-ttu-id="457bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457bb-137">DateTimeOffset</span></span>|<span data-ttu-id="457bb-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="457bb-138">The date and time the object was created.</span></span> <span data-ttu-id="457bb-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="457bb-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="457bb-140">id</span><span class="sxs-lookup"><span data-stu-id="457bb-140">id</span></span>|<span data-ttu-id="457bb-141">String</span><span class="sxs-lookup"><span data-stu-id="457bb-141">String</span></span>|<span data-ttu-id="457bb-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="457bb-142">Key of the entity.</span></span> <span data-ttu-id="457bb-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="457bb-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="457bb-144">value</span><span class="sxs-lookup"><span data-stu-id="457bb-144">value</span></span>|<span data-ttu-id="457bb-145">文字列</span><span class="sxs-lookup"><span data-stu-id="457bb-145">String</span></span>|<span data-ttu-id="457bb-146">関連付けられたプレゼンテーションの文字列型 (string) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="457bb-146">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="457bb-147">応答</span><span class="sxs-lookup"><span data-stu-id="457bb-147">Response</span></span>
<span data-ttu-id="457bb-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="457bb-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="457bb-149">例</span><span class="sxs-lookup"><span data-stu-id="457bb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="457bb-150">要求</span><span class="sxs-lookup"><span data-stu-id="457bb-150">Request</span></span>
<span data-ttu-id="457bb-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="457bb-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="457bb-152">応答</span><span class="sxs-lookup"><span data-stu-id="457bb-152">Response</span></span>
<span data-ttu-id="457bb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="457bb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




