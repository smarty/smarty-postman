# Examples of the Smarty APIs using Postman Collections

---------------------------------------------------- Under Development -------------------------------------------------------

Welcome to [Smarty](https://www.smarty.com), one of the fastest Address Verification and Geocoding services available! 

This repository exists to help you familiarize yourself with the different APIs that Smarty provides through the use of [Postman](https://www.postman.com). More specifically through a [Postman Collection](https://learning.postman.com/docs/collections/collections-overview/). 

This document will act as instructions for the collection, so we recommend opening the collection in a new tab or window.
Click the button below to get started. Once a popup appears asking if you'd like to fork the repository, press the button that says fork.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/26425577-872d9849-4309-44b4-8be5-5a33cd0abdc1?action=collection%2Ffork&collection-url=entityId%3D26425577-872d9849-4309-44b4-8be5-5a33cd0abdc1%26entityType%3Dcollection%26workspaceId%3D04903370-4703-4fcc-83d9-ccfe557f9e37#?env%5BSmarty%20-%20Live%20Deployment%5D=W3sia2V5IjoiYXV0aC1pZCIsInZhbHVlIjoiWU9VUl9BVVRIX19JRCIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJzZWNyZXQiLCJzZXNzaW9uVmFsdWUiOiJiOGNkNzg1Mi00MTlmLTg0MjYtNWNmOC0wYjA0ZDExMDA1ZmMiLCJzZXNzaW9uSW5kZXgiOjB9LHsia2V5IjoiYXV0aC10b2tlbiIsInZhbHVlIjoiWU9VUl9BVVRIX1RPS0VOIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6InNlY3JldCIsInNlc3Npb25WYWx1ZSI6ImQ5TWw3bXBvS1M3Z0VmN2pxRjhhIiwic2Vzc2lvbkluZGV4IjoxfSx7ImtleSI6ImxpY2Vuc2UiLCJ2YWx1ZSI6IllPVVJfTElDRU5TRSIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoidXMtY29yZS1jbG91ZCIsInNlc3Npb25JbmRleCI6Mn0seyJrZXkiOiJ1cmwiLCJ2YWx1ZSI6ImFwaS5zbWFydHlzdHJlZXRzLmNvbSIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiYXBpLnNtYXJ0eXN0cmVldHMuY29tIiwic2Vzc2lvbkluZGV4IjozfSx7ImtleSI6ImlucHV0X2lkIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6NH0seyJrZXkiOiJzdHJlZXQiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4Ijo1fSx7ImtleSI6InN0cmVldDIiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4Ijo2fSx7ImtleSI6InNlY29uZGFyeSIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjd9LHsia2V5IjoiY2l0eSIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjh9LHsia2V5Ijoic3RhdGUiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4Ijo5fSx7ImtleSI6InppcGNvZGUiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4IjoxMH0seyJrZXkiOiJsYXN0bGluZSIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjExfSx7ImtleSI6ImFkcmVzc2VlIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6MTJ9LHsia2V5IjoidXJiYW5pemF0aW9uIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6MTN9LHsia2V5IjoiY2FuZGlkYXRlcyIsInZhbHVlIjoiMTAiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IjEwIiwic2Vzc2lvbkluZGV4IjoxNH0seyJrZXkiOiJtYXRjaCIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjE1fV0=)


