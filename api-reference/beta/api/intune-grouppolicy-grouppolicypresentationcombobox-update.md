---
title: GroupPolicyPresentationComboBox の更新
description: GroupPolicyPresentationComboBox オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04bc5333e8f8fc67a4551708823421b6127862a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985074"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="a7e53-103">GroupPolicyPresentationComboBox の更新</span><span class="sxs-lookup"><span data-stu-id="a7e53-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="a7e53-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7e53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7e53-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e53-106">[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-106">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7e53-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a7e53-107">Prerequisites</span></span>
<span data-ttu-id="a7e53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7e53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7e53-110">Permission type</span></span>|<span data-ttu-id="a7e53-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7e53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7e53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7e53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7e53-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7e53-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7e53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7e53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7e53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7e53-115">Not supported.</span></span>|
|<span data-ttu-id="a7e53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7e53-116">Application</span></span>|<span data-ttu-id="a7e53-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7e53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7e53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7e53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7e53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7e53-119">Request headers</span></span>
|<span data-ttu-id="a7e53-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7e53-120">Header</span></span>|<span data-ttu-id="a7e53-121">値</span><span class="sxs-lookup"><span data-stu-id="a7e53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7e53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7e53-122">Authorization</span></span>|<span data-ttu-id="a7e53-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7e53-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a7e53-124">Accept</span></span>|<span data-ttu-id="a7e53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7e53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7e53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7e53-126">Request body</span></span>
<span data-ttu-id="a7e53-127">要求本文で、 [Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-127">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="a7e53-128">次の表に、 [Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-128">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="a7e53-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7e53-129">Property</span></span>|<span data-ttu-id="a7e53-130">型</span><span class="sxs-lookup"><span data-stu-id="a7e53-130">Type</span></span>|<span data-ttu-id="a7e53-131">説明</span><span class="sxs-lookup"><span data-stu-id="a7e53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e53-132">label</span><span class="sxs-lookup"><span data-stu-id="a7e53-132">label</span></span>|<span data-ttu-id="a7e53-133">String</span><span class="sxs-lookup"><span data-stu-id="a7e53-133">String</span></span>|<span data-ttu-id="a7e53-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="a7e53-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a7e53-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-135">The default value is empty.</span></span> <span data-ttu-id="a7e53-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a7e53-137">id</span><span class="sxs-lookup"><span data-stu-id="a7e53-137">id</span></span>|<span data-ttu-id="a7e53-138">String</span><span class="sxs-lookup"><span data-stu-id="a7e53-138">String</span></span>|<span data-ttu-id="a7e53-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a7e53-139">Key of the entity.</span></span> <span data-ttu-id="a7e53-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a7e53-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e53-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a7e53-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7e53-142">DateTimeOffset</span></span>|<span data-ttu-id="a7e53-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a7e53-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="a7e53-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a7e53-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a7e53-145">defaultValue</span></span>|<span data-ttu-id="a7e53-146">String</span><span class="sxs-lookup"><span data-stu-id="a7e53-146">String</span></span>|<span data-ttu-id="a7e53-147">コンボボックスに表示されるローカライズされた既定の文字列。</span><span class="sxs-lookup"><span data-stu-id="a7e53-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="a7e53-148">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-148">The default value is empty.</span></span>|
|<span data-ttu-id="a7e53-149">助言</span><span class="sxs-lookup"><span data-stu-id="a7e53-149">suggestions</span></span>|<span data-ttu-id="a7e53-150">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a7e53-150">String collection</span></span>|<span data-ttu-id="a7e53-151">コンボボックスのドロップダウンリストに表示されるローカライズされた文字列。</span><span class="sxs-lookup"><span data-stu-id="a7e53-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="a7e53-152">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-152">The default value is empty.</span></span>|
|<span data-ttu-id="a7e53-153">必須</span><span class="sxs-lookup"><span data-stu-id="a7e53-153">required</span></span>|<span data-ttu-id="a7e53-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7e53-154">Boolean</span></span>|<span data-ttu-id="a7e53-155">パラメーターに値を指定する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="a7e53-156">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-156">The default value is false.</span></span>|
|<span data-ttu-id="a7e53-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="a7e53-157">maxLength</span></span>|<span data-ttu-id="a7e53-158">Int64</span><span class="sxs-lookup"><span data-stu-id="a7e53-158">Int64</span></span>|<span data-ttu-id="a7e53-159">パラメーターのテキスト文字の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="a7e53-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="a7e53-160">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="a7e53-161">応答</span><span class="sxs-lookup"><span data-stu-id="a7e53-161">Response</span></span>
<span data-ttu-id="a7e53-162">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a7e53-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7e53-163">例</span><span class="sxs-lookup"><span data-stu-id="a7e53-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7e53-164">要求</span><span class="sxs-lookup"><span data-stu-id="a7e53-164">Request</span></span>
<span data-ttu-id="a7e53-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7e53-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="a7e53-166">応答</span><span class="sxs-lookup"><span data-stu-id="a7e53-166">Response</span></span>
<span data-ttu-id="a7e53-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7e53-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```





