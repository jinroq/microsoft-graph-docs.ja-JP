---
title: groupPolicyPresentationValueMultiText の更新
description: groupPolicyPresentationValueMultiText オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 413d41f0b082c15b717c459311a9805d2a2c1ba2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530558"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="f931e-103">groupPolicyPresentationValueMultiText の更新</span><span class="sxs-lookup"><span data-stu-id="f931e-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="f931e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f931e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f931e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f931e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f931e-106">[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f931e-106">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f931e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f931e-107">Prerequisites</span></span>
<span data-ttu-id="f931e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f931e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f931e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f931e-110">Permission type</span></span>|<span data-ttu-id="f931e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f931e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f931e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f931e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f931e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f931e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f931e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f931e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f931e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f931e-115">Not supported.</span></span>|
|<span data-ttu-id="f931e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f931e-116">Application</span></span>|<span data-ttu-id="f931e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f931e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f931e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f931e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="f931e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f931e-119">Request headers</span></span>
|<span data-ttu-id="f931e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f931e-120">Header</span></span>|<span data-ttu-id="f931e-121">値</span><span class="sxs-lookup"><span data-stu-id="f931e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f931e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f931e-122">Authorization</span></span>|<span data-ttu-id="f931e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f931e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f931e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f931e-124">Accept</span></span>|<span data-ttu-id="f931e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f931e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f931e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f931e-126">Request body</span></span>
<span data-ttu-id="f931e-127">要求本文で、 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f931e-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="f931e-128">次の表に、 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f931e-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="f931e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f931e-129">Property</span></span>|<span data-ttu-id="f931e-130">型</span><span class="sxs-lookup"><span data-stu-id="f931e-130">Type</span></span>|<span data-ttu-id="f931e-131">説明</span><span class="sxs-lookup"><span data-stu-id="f931e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f931e-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f931e-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f931e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f931e-133">DateTimeOffset</span></span>|<span data-ttu-id="f931e-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f931e-134">The date and time the object was last modified.</span></span> <span data-ttu-id="f931e-135">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f931e-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f931e-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f931e-136">createdDateTime</span></span>|<span data-ttu-id="f931e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f931e-137">DateTimeOffset</span></span>|<span data-ttu-id="f931e-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f931e-138">The date and time the object was created.</span></span> <span data-ttu-id="f931e-139">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f931e-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f931e-140">id</span><span class="sxs-lookup"><span data-stu-id="f931e-140">id</span></span>|<span data-ttu-id="f931e-141">String</span><span class="sxs-lookup"><span data-stu-id="f931e-141">String</span></span>|<span data-ttu-id="f931e-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f931e-142">Key of the entity.</span></span> <span data-ttu-id="f931e-143">[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f931e-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f931e-144">values</span><span class="sxs-lookup"><span data-stu-id="f931e-144">values</span></span>|<span data-ttu-id="f931e-145">String collection</span><span class="sxs-lookup"><span data-stu-id="f931e-145">String collection</span></span>|<span data-ttu-id="f931e-146">関連付けられたプレゼンテーションに対して空ではない文字列のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f931e-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="f931e-147">応答</span><span class="sxs-lookup"><span data-stu-id="f931e-147">Response</span></span>
<span data-ttu-id="f931e-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f931e-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f931e-149">例</span><span class="sxs-lookup"><span data-stu-id="f931e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f931e-150">要求</span><span class="sxs-lookup"><span data-stu-id="f931e-150">Request</span></span>
<span data-ttu-id="f931e-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f931e-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f931e-152">応答</span><span class="sxs-lookup"><span data-stu-id="f931e-152">Response</span></span>
<span data-ttu-id="f931e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f931e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```





