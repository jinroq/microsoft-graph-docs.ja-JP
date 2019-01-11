---
title: registryKeyState リソースの種類
description: アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 688c690083e24dc6c8ee7229498910befd0fdf3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804677"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState リソースの種類

アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
|ハイブ|registryHive|[Windows レジストリ ハイブ](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)。 <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\。既定値です。</li></ul> 可能な値は、`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault` です。|
|Key|String|現在の (変更されているなど) のレジストリ キー (ハイブを除く)。|
|oldKey|String|(つまり変更前に) は、以前のレジストリ キー (ハイブを除く)。|
|oldValueData|String|以前の (つまり変更前に) レジストリ キーの値のデータ (内容)。|
|oldValueName|String|以前の (つまり変更前に) レジストリ キーの値の名前。|
|操作​​|registryOperation|レジストリ キーの名前または値を変更する操作です。 可能な値は、`unknown`、`create`、`modify`、`delete` です。|
|プロセス Id|Int32|(プロセスのアラート 'プロセス' コレクションの詳細が表示されます) のレジストリ キーを変更するプロセスの ID (PID) を処理します。|
|セグ|String|現在 (つまり変更されている) のレジストリ キーの値のデータ (内容)。|
|値名|String|現在の (変更されているなど) のレジストリ キー値の名前|
|valueType|registryValueType|[レジストリ キーの値の型](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>定義</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> 可能な値は、`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
